# pdftowiki
extension that allows users to convert pdf documents to wiki pages


# flow draft
1. User goes to special page to upload PDF file
2. User fills out form with namespace, categories, target page title (other?)
3. Extension stores the PDF temporarily
4. Special page triggers python conversion - call script inside container
5. Python converts PDF -> HTML -> Parsoid -> WikiText
6. Extension receives converted text
7. Extension injects it into a preloaded edit session
8. User is redirected to edit session (visual editor) for review/editing
9. User clicks save - and should be notified if they try to click away without saving