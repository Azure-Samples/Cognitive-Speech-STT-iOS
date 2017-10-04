# Microsoft Speech API: iOS Speech-to-Text Client Library and Samples

This repo contains the iOS client library and samples for Speech-to-Text in Microsoft Speech API, an offering within [Microsoft Cognitive Services on Azure](https://azure.microsoft.com/en-us/services/cognitive-services/), formerly known as Project Oxford.

* [Learn about the Speech API](https://azure.microsoft.com/en-us/services/cognitive-services/speech/)
* [Read the documentation](https://docs.microsoft.com/en-us/azure/cognitive-services/speech/home)
* [Find more SDKs & Samples](https://www.microsoft.com/cognitive-services/en-us/SDK-Sample?api=bing%20speech)

## The Client Library

To add the Speech Client Library dependency to an existing XCode Project:

1. Select your target application, and open the menu `File` then `Add Files to ...`
2. Navigate to `iPhoneOS`, select `SpeechSDK.framework`, and click `Add`.
3. Go to your project settings, by single clicking your project, and navigate to the `General` tab.  You will notice that SpeechSDK.framework exists under the `Linked Frameworks and Libraries` section.
4. In the `General` tab, under the `Embedded Binaries` section, click the (+) button.   In the dialog, select `SpeechSDK.framework` and click the `Add` button.
5. If you wish to run on the iOS Simulator or MacOSX, repeat steps 2-4 but choose either `iPhoneSimulator` or `MacOSX` instead.

The Client Library Reference for iOS can be found [here](https://cdn.rawgit.com/Microsoft/Cognitive-Speech-STT-iOS/master/com.Microsoft.SpeechSDK-1_0-for-iOS.docset/Contents/Resources/Documents/index.html).

## The Sample

This sample demonstrates the following features using a wav file or external microphone input:

* Short-form recognition
* Long-form dictation
* Recognition with intent

### Build the sample

1. First, you must obtain a Speech API subscription key by following the instructions on [Subscriptions](https://azure.microsoft.com/en-us/try/cognitive-services/).
2. Start XCode and choose the menu `File`, and `Open...` the workspace file `Cognitive-Speech-STT-iOS > SpeechSDK.xcworkspace`.
3. Use one of your subscription keys as the primaryKey in `Samples/SpeechRecognitionServerExample/settings.plist`.
4. If you want to use *Recognition with intent*, you also need to sign up for [Language Understanding Intelligent Service (LUIS)](https://azure.microsoft.com/en-us/services/cognitive-services/language-understanding-intelligent-service/) and set the key values in `luisAppID` and `luisSubscriptionID` in `Samples/SpeechRecognitionServerExample/settings.plist`.
5. In XCode, select menu `Product > Build` to build the sample and `Run` to launch the sample app.

### Running the sample
In XCode, select the menu `Product`, and `Run` to launch this sample app.

1. In the application, press the button `Change Mode` to select which recognition mode you would like to use.
2. To Start recognition, press the Start button.

<img src="SampleScreenshots/SampleRunning1.png" width="50%"/>

## Contributing

We welcome contributions. Feel free to file issues and pull requests on the repo and we'll address them as we can. Learn more about how you can help on our [Contribution Rules & Guidelines](</CONTRIBUTING.md>).

You can reach out to us anytime with questions and suggestions using our communities below:

* **Support questions:** [StackOverflow](<https://stackoverflow.com/questions/tagged/microsoft-cognitive>)
* **Feedback & feature requests:** [Cognitive Services UserVoice Forum](<https://cognitive.uservoice.com>)

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information, see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## License

All Microsoft Cognitive Services SDKs and samples are licensed with the MIT License. For more information, see
[LICENSE](</LICENSE.md>).

Sample images are licensed separately, please refer to [LICENSE-IMAGE](</LICENSE-IMAGE.md>).

## Developer Code of Conduct

Developers using Cognitive Services, including this client library and sample, are expected to follow the "Developer Code of Conduct for Microsoft Cognitive Services", found at [http://go.microsoft.com/fwlink/?LinkId=698895](http://go.microsoft.com/fwlink/?LinkId=698895).
