# SocialWorker

![SocialWorker](https://qiita-image-store.s3.amazonaws.com/0/98018/dc39c8a8-ae3b-5323-d953-3b97e5a8cfa4.png)

SocialWorkerは、Twitter、Facebook、Line、Instagram、メールへの連携を簡単に行うことが出来るUnityAssetです。
詳しくは以下をご確認下さい。

[Japanese](https://github.com/)/[English](https://github.com/)

## Requirement

### iOS
iOS 6.0以上

### Android
Android 2.3以上

## Usage

    SocialWorker.PostTwitter(string message, string url, string imagePath, Action<SocialWorkerResult> onResult = null)
    SocialWorker.PostFacebook(string imagePath, Action<SocialWorkerResult> onResult = null)
    SocialWorker.PostLine(string message, string imagePath, Action<SocialWorkerResult> onResult = null)
    SocialWorker.PostInstagram(string imagePath, Action<SocialWorkerResult> onResult = null)
    SocialWorker.PostMail(string[] to, string[] cc, string[] bcc, string subject, string message, string imagePath, Action<SocialWorkerResult> onResult = null)
    SocialWorker.CreateChooser(string message, string imagePath, Action<SocialWorkerResult> onResult = null)

## Author

[yedo-factory](http://yedo-factory.co.jp/)
