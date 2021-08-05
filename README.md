# 🇵🇹 COVID-19 Digital Certificate template for Apple Wallet

Based on [this document](https://developer.apple.com/library/archive/documentation/UserExperience/Conceptual/PassKit_PG/YourFirst.html) from Apple's developer guide.

## Creating your pass:

1. Fill in the fields marked as `<<< FILL ME (...) >>>` in `pass.json`;
2. Use `signpass` with the invocation `./signpass -p path/to/pass.pass` to sign your pass. `signpass`'s source can be acquired [here](https://developer.apple.com/services-account/download?path=/iOS/Wallet_Support_Materials/WalletCompanionFiles.zip);
3. Install the generated `.pkpass` file on your device!

## Extracting QR code data:

1. Install `zbarimg` (`brew install zbarimg`);
2. Run `screencapture -i $TMPDIR/screencapture.bmp && zbarimg -q --raw $TMPDIR/screencapture.bmp | pbcopy`;
3. The QR code data should now be in your clipboard, ready to be pasted into `barcode.image`!

## License / Disclaimer

The pass source is published under a MIT license.

The syringe image is part of Samsung's emojis.

The SNS logo is property of `Governo da República Portuguesa - Ministério da Saúde`.