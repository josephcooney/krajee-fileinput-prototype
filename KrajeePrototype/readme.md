# Demonstration of krajee file preview plugin, PDF Preview, and avoiding CORS issues on Safari on iOS

https://plugins.krajee.com/file-preview-management-demo

Here is where the PDF preview using viewer.html is specified https://plugins.krajee.com/file-preview-management-demo#preview-pdf

    <div class="file-loading">
        <input id="file-kv-pdf" name="file-kv-pdf[]" type="file" multiple>
    </div>
    <script>
    $('#file-kv-pdf').fileinput({
        uploadUrl: "/file-upload-batch/1",
        pdfRendererUrl: 'https://plugins.krajee.com/pdfjs/web/viewer.html',
        overwriteInitial: false,
        initialPreviewAsData: true,
        initialPreview: [
            'https://plugins.krajee.com/samples/sample-2.pdf'
        ],
        initialPreviewConfig: [
            {type: 'pdf', description: "<h5>PDF File One</h5> This is a representative placeholder description number one for this PDF file.", size: 3072}
        ]
    });
    </script>