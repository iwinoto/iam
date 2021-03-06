---

copyright:

  years: 2015, 2018
lastupdated: "2018-05-02"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# サービス ID のアクセス・ポリシーの管理
{: #serviceidpolicy}

サービス ID を作成する際にそのサービス ID のサービス・ポリシーを割り当てて、そのサービス ID がサービスの認証に使用される時に許可されるアクセス・レベルを制御することができます。 これらの割り当てられたアクセス・ポリシーは、既存のポリシーを変更したり、ポリシーを削除したり、新しいポリシーを割り当てたりして、いつでも更新することができます。

**注**: 現在使用しているサービス ID の既存のポリシーを削除したり編集したりすると、サービスが中断されることがあります。

## 新規アクセス権限の割り当て

リソース・グループ内のすべてのリソースへのアクセス権限、または、リソース・グループ内の 1 つのサービスのみへのアクセス権限を割り当てるには、以下の手順を実行します。

1. メニュー・バーで、**「管理」** &gt; **「セキュリティー」** &gt; **「ID およびアクセス」** &gt; **「サービス ID」**とクリックします。
2. サービス・ポリシーを割り当てるサービス ID を表から選択します。
3. **「アクセス権限の割り当て (Assign access)」**をクリックします。
4. **「リソース・グループによる割り当て (Assign by resource group)」**を選択します。
5. リソース・グループを選択します。
6. **「リソース・グループへのアクセス権限の割り当て (Assign access to resource group)」**フィールドで役割を選択します。 このオプションは、ユーザーがダッシュボードでのリソース・グループの表示、リソース・グループ名の編集、またはグループへのユーザー・アクセスの管理を行うことを許可します。 指定するリソースへのアクセス権限のみをユーザーに付与し、そのリソースが割り当てられているグループへのアクセス権限は付与しない場合は、**「アクセス権限なし」**を選択できます。
7. リソース・グループ内のいずれかのサービスを選択するか、または、選択したグループ内のすべてのサービスへのアクセス権限を提供することを選択します。
8. 必要なアクセス権限をユーザーに割り当てるため、役割の任意の組み合わせを選択します。 このアクセス権限は、ポリシーに選択したリソースにのみ適用されます。 リソース・グループである実際のコンテナーへのアクセス権限は付与されません。
9. **「割り当て」**を選択します。

アカウント内の個別リソースへのアクセス権限を割り当てるには、以下の手順を実行します。

1. メニュー・バーで、**「管理」** &gt; **「セキュリティー」** &gt; **「ID およびアクセス」** &gt; **「サービス ID」**とクリックします。
2. サービス・ポリシーを割り当てるサービス ID を表から選択します。
3. **「アクセス権限の割り当て (Assign access)」**をクリックします。
4. **「リソースによる割り当て (Assign by resource)」**を選択します。
5. サービスを選択します。
6. プロンプトが出されたら、**「すべての現行地域」**、または特定の地域を選択します。
7. **「すべての現行サービス・インスタンス」**を選択するか、特定のサービス・インスタンスを選択します。
8. 選択したサービスに応じて、以下のフィールドが表示される場合があります。 これらのフィールドの値を入力しないと、ポリシーの割り当ては、バケット・レベルではなく、サービス・インスタンス・レベルで行われます。
    * **リソース・タイプ**: **「バケット」** を入力します。
    * **リソース ID**: バケットの名前を入力します。
9. 必要なアクセス権限をユーザーに割り当てるため、役割の任意の組み合わせを選択します。
10. **「割り当て」**を選択します。



## 既存のアクセス権限の編集

既存のポリシーを編集するには、以下のようにします。

1. メニュー・バーで、**「管理」** &gt; **「セキュリティー」** &gt; **「ID およびアクセス」** &gt; **「サービス ID」**とクリックします。
2. サービス・ポリシーを編集するサービス ID を表から選択します。
3. 編集するポリシーの行を識別し、**「アクション」**メニューから**「ポリシーの編集」**を選択します。
4. 変更を行い、ポリシーを保存します。

## アクセス権限の削除

既存のポリシーを削除するには、以下のようにします。

1. メニュー・バーで、**「管理」** &gt; **「セキュリティー」** &gt; **「ID およびアクセス」** &gt; **「サービス ID」**とクリックします。
2. サービス・ポリシーを削除するサービス ID を表から選択します。
3. 削除するポリシーの行を識別し、**「アクション」**メニューから**「削除」**を選択します。
4. 削除しようとしているポリシーの詳細を検討し、確認のために**「削除」**をクリックします。
