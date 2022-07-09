# k8s_ArgoCD

## 手順

1. [ここ](https://github.com/argoproj/argo-cd/blob/master/docs/getting_started.md)を参考にArgoCDをインストール

2. localhost:8080でArgoCDのUI画面を開きログインする  
※brew install argocdをインストールしないとエラー出ることもあった
   
3. 左上のNEW APPから作成する（下記画像を参考）

<img width="851" alt="1" src="https://user-images.githubusercontent.com/63485252/178106262-46251697-9aa8-4444-9f28-677e24e4d61f.png">
<img width="882" alt="2" src="https://user-images.githubusercontent.com/63485252/178106265-4ab7a8ff-d02a-49ea-a606-23ed62fb24b9.png">

4. mainブランチを更新すると自動で展開される


## コマンド一覧

`kubectl get svc -n k8s-demo`
`kubectl get pods -n k8s-demo`
`kubectl get svc -n argocd`
`kubectl delete -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/core-install.yaml`
