---
############################# Static ############################
layout: "auto-gen"
date: 2021-09-22T14:22:14+03:00
draft: false
product_tag: total
platform_tag: net

############################# Head ############################
head_title: "Add Barcodes to PDF Document in Java"
head_description: "Add 65+ barcode images to PDF file in Java & J2SE platforms in your desktop, web or mobile applications."

############################# Header ############################
title: "Add Barcodes to PDF File in Java"
description: "Add 1D & 2D Barcode images to PDF file in Java applications. Programmatically integrate 65+ popular barcode symbologies including QR Code, PDF 417, GS1 DataBar, Data Matrix, ISBN, MSI, Postal, UPCA, Aztec etc in your documents with the capabilities to control the barcode size and formatting settings by adding a few line of code."

############################# SubMenu ############################
submenu:
    enable: false

############################# About ############################
about:
    enable: false
    title: "About GroupDocs.Total for .NET"
    content: |
        GroupDocs.Total for .NET is a suite of document manipulation APIs to perform powerful documents manipulation & automation features within your desktop solutions and web apps without requiring any other commercial application. It enables developers to add the functionalities (view, edit, annotate, convert, compare, e-sign, assemble, search, parse, merge, redact and classify) within PDF, Microsoft Office Word, Excel, PowerPoint, OneNote, Visio, Outlook, HTML, images, graphics, diagrams and 90+ other popular document formats.

        GroupDocs.Total APIs are well supported on all major operating systems and platforms including .NET Framework, .NET Standard, .NET Core, Mono and Xamarin.

############################# Steps ############################
steps:
    enable: true
    title_left: "Java Code to Add Barcodes to PDF"
    content_left: |
        [Conholdate.Total for Java](https://products.conholdate.com/total/java/) makes it easy for Java developers to generate customized barcode images based on provided text, and dynamically add it to the PDF document by implementing a few easy steps.

        *   Instantiate linear barcode object, Set the Code text and symbology type for the barcode
        *   Creating memory stream and Saving barcode image to memory stream
        *   Create PDF document and add a section to the PDF document
        *   Create **PdfFileMend** object to add barcode image
        *   Bind PDF document with the **PdfFileMend** object
        *   Add image in the PDF file
        
    title_right: "Generate Barcodes in PDF Document"
    content_right: |
        The following piece of code requires `Aspose.PDF` & `Aspose.BarCode` namespaces. You can get the respective files from the [downloads](https://downloads.conholdate.com/total/java) or fetch the whole package from [Maven](https://repository.conholdate.com/webapp/#/artifacts/browse/tree/General/repo) to add 'Conholdate.Total` directly in your workspace.

        Draw barcode to a PDF document in Java on different operating systems such as Windows, Linux or macOS while using platforms such as Windows Azure, Mono and Xamarin.
        
    code: |
        ```cs {linenos=false}
        // Instantiate linear barcode object, Set the Code text and symbology type for the barcode
        BarcodeGenerator generator = new BarcodeGenerator(EncodeTypes.CODE_39_STANDARD, "1234567");
        generator.save(dataDir + "barcodeToPDF.bmp", BarCodeImageFormat.bmp);

        InputStream in = new FileInputStream(dataDir + "barcodeToPDF.bmp");

        // Create a PDF document and Add a section to the PDF document
        Document doc = new Document();
        doc.getPages().add();

        // Open document
        PdfFileMend mender = new PdfFileMend();

        // Create PdfFileMend object to add Barcode image
        mender.bindPdf(doc);

        // Add image in the PDF file
        mender.addImage(in, 1, 100, 600, 200, 700);

        // Save changes
        mender.save(dataDir + "AddImage_out.pdf");

        // Close PdfFileMend object
        mender.close();
        ```
        
############################# Demos ############################
demos:
    enable: false
    title: "Free Document Automation Apps"
    content: |
        Offline [GroupDocs.Total Apps](https://products.groupdocs.app/total) to view, convert, annotate, compare, sign, assemble, parse, classify, redact and search documents.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pdf-o"
          title: " About PDF File Format"
          content: |
            Portable Document Format (PDF) is a type of document created by Adobe back in 1990s. The purpose of this file format was to introduce a standard for representation of documents and other reference material in a format that is independent of application software, hardware as well as Operating System. The PDF file format has full capability to contain information like text, images, hyperlinks, form-fields, rich media, digital signatures, attachments, metadata, Geospatial features and 3D objects in it that can become as part of source document. In most of the cases, existing documents are converted to PDF rather than creating a new PDF from scratch. But that doesn’t mean there are no software for creation or manipulation of PDF files.

          link: "https://docs.fileformat.com/pdf/"

############################# More Formats ############################
more_formats:
    enable: false
    title: "Insert barcodes to Other Documents"
    format: 
        # format loop
        - name: "Add Barcode to PDF"
          link: "https://products.conholdate.com/total/net/barcode/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add Barcode to Word"
          link: "https://products.conholdate.com/total/net/barcode/word/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add Barcode to Excel"
          link: "https://products.conholdate.com/total/net/barcode/excel/"
          description: "Microsoft Excel Worksheet"

        # format loop
        - name: "Add Barcode to DOC"
          link: "https://products.conholdate.com/total/net/barcode/doc/"
          description: "Microsoft Word 97 – 2007 Document"

        # format loop
        - name: "Add Barcode to DOT"
          link: "https://products.conholdate.com/total/net/barcode/dot/"
          description: "Microsoft Word 97 – 2007 Template"

        # format loop
        - name: "Add Barcode to DOCX"
          link: "https://products.conholdate.com/total/net/barcode/docx/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add Barcode to DOCM"
          link: "https://products.conholdate.com/total/net/barcode/docm/"
          description: "XML Macro-Enabled Document"

        # format loop
        - name: "Add Barcode to DOTX"
          link: "https://products.conholdate.com/total/net/barcode/dotx/"
          description: "Microsoft Word Template"

        # format loop
        - name: "Add Barcode to DOTM"
          link: "https://products.conholdate.com/total/net/barcode/dotm/"
          description: "XML Macro-Enabled Template"

        # format loop
        - name: "Add Barcode to ODT"
          link: "https://products.conholdate.com/total/net/barcode/odt/"
          description: "OpenDocument Text File"

        # format loop
        - name: "Add Barcode to OTT"
          link: "https://products.conholdate.com/total/net/barcode/ott/"
          description: "OpenDocument Text Template"

        # format loop
        - name: "Add Barcode to XLS"
          link: "https://products.conholdate.com/total/net/barcode/xls/"
          description: "Microsoft Excel 95-2003 Worksheet"

        # format loop
        - name: "Add Barcode to XLSX"
          link: "https://products.conholdate.com/total/net/barcode/xlsx/"
          description: "Microsoft Excel Worksheet"

        # format loop
        - name: "Add Barcode to XLSB"
          link: "https://products.conholdate.com/total/net/barcode/xlsb/"
          description: "Excel Binary Workbook"

        # format loop
        - name: "Add Barcode to XLSM"
          link: "https://products.conholdate.com/total/net/barcode/xlsm/"
          description: "Excel Macro-Enabled Workbook"

        # format loop
        - name: "Add Barcode to XLTM"
          link: "https://products.conholdate.com/total/net/barcode/xltm/"
          description: "Excel Macro-Enabled Template"

        # format loop
        - name: "Add Barcode to XLT"
          link: "https://products.conholdate.com/total/net/barcode/xlt/"
          description: "Microsoft Excel 97-2003 Template"

        # format loop
        - name: "Add Barcode to XLTX"
          link: "https://products.conholdate.com/total/net/barcode/xltx/"
          description: "Excel Open XML Spreadsheet Template"

        # format loop
        - name: "Add Barcode to CSV"
          link: "https://products.conholdate.com/total/net/barcode/csv/"
          description: "Comma Separated Values File"

        # format loop
        - name: "Add Barcode to TSV"
          link: "https://products.conholdate.com/total/net/barcode/tsv/"
          description: "Tab-separated Values File"

        # format loop
        - name: "Add Barcode to ODS"
          link: "https://products.conholdate.com/total/net/barcode/ods/"
          description: "OpenDocument Spreadsheet"

        # format loop
        - name: "Add Barcode to HTML"
          link: "https://products.conholdate.com/total/net/barcode/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Add Barcode to MOBI"
          link: "https://products.conholdate.com/total/net/barcode/mobi/"
          description: "Mobipocket e-book format"

        # format loop
        - name: "Add Barcode to EPUB"
          link: "https://products.conholdate.com/total/net/barcode/epub/"
          description: "Digital E-Book File Format"

        # format loop
        - name: "Add Barcode to TIFF"
          link: "https://products.conholdate.com/total/net/barcode/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add Barcode to JPEG"
          link: "https://products.conholdate.com/total/net/barcode/jpeg/"
          description: "Joint Photographic Experts Group"

        # format loop
        - name: "Add Barcode to PNG"
          link: "https://products.conholdate.com/total/net/barcode/png/"
          description: "Portable Network Graphics"

        # format loop
        - name: "Add Barcode to BMP"
          link: "https://products.conholdate.com/total/net/barcode/bmp/"
          description: "Bitmap Picture"

        # format loop
        - name: "Add Barcode to SVG"
          link: "https://products.conholdate.com/total/net/barcode/svg/"
          description: "Scalable Vector Graphics Format"

        # format loop
        - name: "Add Barcode to GIF"
          link: "https://products.conholdate.com/total/net/barcode/gif/"
          description: "Graphics Interchange Format"

        # format loop
        - name: "Add Barcode to EMF"
          link: "https://products.conholdate.com/total/net/barcode/emf/"
          description: "Windows Enhanced Metafile"

        # format loop
        - name: "Add Barcode to PCL"
          link: "https://products.conholdate.com/total/net/barcode/pcl/"
          description: "Printer Control Language"

############################# Back to top ###############################
back_to_top:
  enable: true
---