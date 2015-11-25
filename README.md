# SocialWorker

![SocialWorker](https://qiita-image-store.s3.amazonaws.com/0/98018/dc39c8a8-ae3b-5323-d953-3b97e5a8cfa4.png)

SocialWorkerは、iOS/AndroidでのTwitter、Facebook、Line、Instagram、メールへの連携を簡単に行うことが出来るUnityAssetです。  
詳しくは以下をご確認下さい。

[Japanese](https://github.com/)/[English](https://github.com/)

## Description

SocialWorkerは各種SNSへの簡単なデータの受け渡しをサポートしています。そのため、連携可能なデータはメッセージと画像のみです(SNSによっては微妙に追加で渡せるデータもあったりしますが)。  
連携方法は、iOSではURLSchemeを主に使用しており、AndroidではIntentによるデータの受け渡しの方法を取っています。  

## Requirement

iOS 6.0+  
Android 2.3+

## Usage

1. SocialWorker Prefab の設置

[SocialWorker/Prefabs/SocialWorker]をHierarchyに設置。

2. スクリプトから連携メソッドを呼ぶ

    SocialWorker.PostTwitter(string message, string url, string imagePath, Action<SocialWorkerResult> onResult = null)
    SocialWorker.PostFacebook(string imagePath, Action<SocialWorkerResult> onResult = null)
    SocialWorker.PostLine(string message, string imagePath, Action<SocialWorkerResult> onResult = null)
    SocialWorker.PostInstagram(string imagePath, Action<SocialWorkerResult> onResult = null)
    SocialWorker.PostMail(string[] to, string[] cc, string[] bcc, string subject, string message, string imagePath, Action<SocialWorkerResult> onResult = null)
    SocialWorker.CreateChooser(string message, string imagePath, Action<SocialWorkerResult> onResult = null)

## Author

[yedo-factory](http://yedo-factory.co.jp/)
