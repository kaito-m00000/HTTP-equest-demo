//この表記があるところは予定とする。

Local
    とりあえずLocalで書いたNodeJSを
    CloudRunにデプロイしてみる
    デプロイ後、閉じて改めてGithubにアップロード
    参考 1：GoogleCloud Run. "Cloud Run に Node.js サービスをデプロイする" 2023-07-21 UTC.  
    https://cloud.google.com/run/docs/quickstarts/build-and-deploy/deploy-nodejs-service?hl=ja
    参照日 2023-07-23 JST

↓
git
↓
Cloud Build
↓
    Localで書いたコードをGitにアップロードし、
    Kubernates engineで管理することをみこして
    CloudBuildでコンテナを作成する。
    コンテナに基づいてデプロイするため、
    Cloud Build から　Gitのソースをコンテナ化して、
    CloudRunの継続的デプロイを実現する。

    参考 2：GoogleCloud　Build. "GitHub からのリポジトリのビルド" 2023-07-20 UTC. 
    https://cloud.google.com/build/docs/automating-builds/github/build-repos-from-github?hl=ja
    参照日 2023-07-24 JST  
    参考 3：GoogleCloud Run. "Cloud Build を使用した Git からの継続的なデプロイ" 2023-07-20 UTC.
    https://cloud.google.com/run/docs/continuous-deployment-with-cloud-build?hl=ja
    参照日 2023-07-24 JST

    //Kubernetes
    //↓

Cloud Run

    おまけ：CloudRunにカスタムドメインを紐付けてみた。
    demo1.programegg.app
