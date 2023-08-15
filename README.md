# Qrcode_generator
To generator the Qr Code using python


    import qrcode

    url=input("Enter the url:")
    path=input("Enter the name of file to save Qr Code (extension.png):")
    features=qrcode.QRCode(version=1,box_size=40,border=3)
    features.add_data(url)
    features.make(fit=True)
    generator_image=features.make_image(fill_color="black",back_color="white")
    generator_image.save(path)
