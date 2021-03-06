# LRC Editor &nbsp; [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Version: 3.2.4](https://d25lcipzij17d.cloudfront.net/badge.svg?id=gh&type=6&v=3.2.4)

<img src="https://i.stack.imgur.com/KSovE.png" alt="LRC Editor App Icon" align="left" style="margin: 10px 20px 10px 10px; border-radius: 15%; box-shadow: 0 6px 20px 2px black">

LRC Editor is an Android app that helps you to create and edit .lrc files easily

It is available to download on the [Google Play Store][play_store_page], [F-Droid][fdroid_page] as well as [GitHub][github_release_page].

<p>
	<a href="https://play.google.com/store/apps/details?id=com.cg.lrceditor">
		<img src="https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png" alt="Download from Google Play" height="80px">
	</a>
	<a href="https://f-droid.org/packages/com.cg.lrceditor/">
		<img src="https://fdroid.gitlab.io/artwork/badge/get-it-on.png" alt="Get it on F-Droid" height="80px">
	 </a>
	<a href="https://github.com/Spikatrix/LRC-Editor/releases">
		<img src="https://i.stack.imgur.com/S4MQt.png" alt="Download from GitHub" height="80px">
	</a>
</p>

## About

LRC Editor is a small, minimal Android app that helps you to create and edit .lrc (lyric) files. It's got all the necessary features required to edit LRC files easily. Timestamps can be both fine and coarse tuned. You can edit lyrics, insert more lyrics, batch edit timestamps and much more. Also, you can open LRC files directly from your file manager<sup>1</sup>. The best part is that LRC Editor is completely free of ads!

You can then use the LRC files in Karaoke applications, Music players etc that support it. The stock music players of major phone manufacturers like Xiaomi, Huawei, OPPO, Samsung and more support LRC files. LRC files aren't supported on LG's stock media player, the Google Play Music app among others.

**Note**: To get the best precision from this app, use a high quality constant bitrate MP3 file or another music container that isn't compressed and is designed for precise seeking. Compressed music files usually don't have accurate seek information in them which might lead to desync issues.

<sup>1</sup> [Samsung's stock file manager has issues with this](https://github.com/Spikatrix/LRC-Editor/issues/16)

## Screenshots

<img src="https://raw.githubusercontent.com/Spikatrix/LRC-Editor/master/fastlane/metadata/android/en-US/images/phoneScreenshots/1.png" height="300px"> &nbsp; &nbsp; <img src="https://raw.githubusercontent.com/Spikatrix/LRC-Editor/master/fastlane/metadata/android/en-US/images/phoneScreenshots/3.png" height="300px">

More screenshots are available in the [Google Play Store page][play_store_page]

## Permissions

LRC Editor requires the storage permission so that it can read and save LRC files.

Note: Android 11 brings much more stricter storage access enforcements and LRC Editor might not be able to access storage even after granting the storage permission.

## Build from source

If you wish to build from source, clone the repo and run gradle's `assembleDebug` task:

	$ git clone https://github.com/Spikatrix/LRC-Editor
	$ cd LRC-Editor
	$ ./gradlew assembleDebug

(Use `gradlew.bat` if you're on Windows)

Alternatively, you can clone the repo and open the project in Android Studio and then build the app from there.

There are two build flavors in this project:
 - `fdroid`: The build for [F-Droid][fdroid] which has links to LRC Editor's F-Droid page and no IAP implementation.
 - `playstore`: The build for [Google Play Store][play_store] which has links to LRC Editor's Play store page and has an IAP implementation. However, the IAPs will not work as the original keys are not exposed.

## Contributing

LRC Editor is a FOSS app developed by [me](https://github.com/Spikatrix). Contributions are always welcome.

Here are a few ways you can help:
 * Report bugs via the [Issue Tracker][issue_tracker] and suggestions via [email][email_feedback]
 * [Translate the app][translate_app] and send in the translations via a pull request or via [email][email_app_translation]
 * Translate the app's [Google Play Store description][play_store_page] and send it to me via [email][email_play_store_translation]
 * Tackle one of the issues/feature-requests from the [Issue Tracker][issue_tracker], make new useful features or fix bugs. In doing so, make sure that the app is still fast, minimal and easy to use.
 * Cleanup and refactor the code making it much more easier to understand and maintain.

## Translators

A big thank you to all the app translators:
 - Chinese (zh-rTW) by Martin C
 - German (de) by Leon Thelen
 - Indonesian (in) by Fajar Maulana
 - Polish (pl) by Zbigniew Zienko
 - Portuguese (pt-rBR) by Ayrtown Karlos

And a big thank you to all the Google Play Store description translators:
 - German (de) by Leon Thelen
 - Portuguese (pt-rBR) by Ayrtown Karlos


## License

This project is licensed under the [GNU GPLv3 License][project_license]

<!-- Link references -->
[play_store_page]: https://play.google.com/store/apps/details?id=com.cg.lrceditor
[fdroid_page]: https://f-droid.org/packages/com.cg.lrceditor
[github_release_page]: https://github.com/Spikatrix/LRC-Editor/releases

[play_store]: https://play.google.com/store
[fdroid]: https://www.f-droid.org/

[issue_tracker]: https://github.com/Spikatrix/LRC-Editor/issues
[translate_app]: https://github.com/Spikatrix/LRC-Editor/blob/master/app/src/main/res/values/strings.xml

[email_feedback]: mailto:cg.devworks@gmail.com?subject=LRC+Editor+Feedback&body=Your+feedback+here
[email_app_translation]: mailto:cg.devworks@gmail.com?subject=LRC+Editor+Translation
[email_play_store_translation]: mailto:cg.devworks@gmail.com?subject=LRC+Editor+Play+Store+Translation

[project_license]: https://github.com/Spikatrix/LRC-Editor/blob/master/LICENSE
