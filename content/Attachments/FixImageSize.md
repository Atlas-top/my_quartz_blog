<%*
// 获取当前选中的文字
let selection = tp.file.selection();

// 匹配标准 Markdown 图片语法：![](path) 或 ![]( <path> )
// 兼容你截图中的 < > 和 空格
let match = selection.match(/!\[\]\(\s*<?([^>\s]+)>?\s*\)/);

if (match) {
    let imagePath = match[1];
    // 这里默认设置为 400，你可以根据喜好修改这个数字
    let replacement = `<img src="${imagePath}" width="400">`;
    
    // 替换选中的内容
    const activeView = app.workspace.getActiveViewOfType(obsidian.MarkdownView);
    if (activeView) {
        const editor = activeView.editor;
        editor.replaceSelection(replacement);
    }
} else {
    new Notice("未识别到有效的图片链接，请确保选中了完整的 ![]() 语法");
}
-%>