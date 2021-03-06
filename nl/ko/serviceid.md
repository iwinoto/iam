---

copyright:

  years: 2017, 2018
lastupdated: "2018-03-19"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# 서비스 ID 작성 및 관리
{: #serviceids}

서비스 ID는 사용자 ID가 사용자를 식별하는 방법과 비슷하게 서비스 또는 애플리케이션을 식별합니다. 작성한 서비스 ID를 사용하여 {{site.data.keyword.Bluemix_notm}} 서비스에 대해 {{site.data.keyword.Bluemix_notm}} 액세스 외부에서 애플리케이션을 사용하도록 설정할 수 있습니다. 특정 서비스 사용을 위해 권한을 제한하거나 여러 서비스에 액세스하기 위해 권한을 결합하는 특정 액세스 정책을 서비스 ID에 지정할 수 있습니다. 서비스 ID는 특정 사용자에게 묶여 있지 않으므로, 사용자가 우연히 조직을 나가게 되어 계정에서 삭제되는 경우에도 서비스 ID는 남게 되어 애플리케이션 또는 서비스가 유지되고 실행됩니다.

서비스 ID를 작성하는 경우 UI에서 식별하고 작업하기 쉬운 고유 이름 및 설명을 작성합니다. 서비스 ID를 작성하면, 애플리케이션에서 {{site.data.keyword.Bluemix_notm}} 서비스 인증에 사용할 수 있는 각 서비스 ID에 특정한 API 키를 작성할 수 있습니다. 애플리케이션에 {{site.data.keyword.Bluemix_notm}} 서비스 인증에 적합한 액세스 권한이 있는지 확인하기 위해, 작성하는 각 서비스 ID에 지정된 서비스 정책을 사용합니다.

서비스 ID와 연관된 액세스 정책은 해당 서비스 ID가 특정 서비스에 액세스하는 데 사용되는 경우 수행할 수 있는 특정 조치를 사용합니다. 단일 서비스 ID에는 여러 ID와 액세스 사용 서비스 및 심지어 단일 서비스의 서로 다른 인스턴스에 액세스하는 경우 허용되는 액세스 레벨을 정의하는 여러 정책이 지정될 수 있습니다. 예를 들어, 각각 두 개의 서비스 인스턴스가 있는 두 개의 서비스가 있습니다. 예를 들어, 한 서비스의 사용 가능한 모든 인스턴스에 `뷰어` 역할을 지정하고 두 번째 서비스에 대한 하나의 인스턴스에만 `편집자` 역할을 지정할 수 있습니다. 이와 같이 여러 서비스에 대한 액세스를 사용자 정의할 수 있지만 전체에 대한 인증에 단일 API 키를 사용할 수 있습니다.


## 서비스 ID 작성

서비스 ID를 작성하려면 **관리** &gt; **보안** &gt; **ID 및 액세스**로 이동한 후에 사이드 패널에서 **서비스 ID**를 선택하십시오. 프로세스에 따라 서비스 ID의 이름과 설명을 작성하십시오. 그런 다음 **조치** 메뉴를 사용하여 서비스 ID를 관리하십시오. 정책을 지정하고 API 키를 작성하여 시작할 수 있습니다. API 키를 사용한 작업에 대한 자세한 정보는 [서비스 ID API 키 관리](/docs/iam/serviceid_keys.html#serviceidapikeys)를 참조하십시오. 서비스 ID 관리에 사용되는 CLI 명령에 대한 세부사항은 [API 키 및 정책 관리를 위한 명령](/docs/cli/reference/bluemix_cli/bx_cli.html#bx_commands_iam)을 참조하십시오.

## 서비스 ID 업데이트

언제든 이름 및 설명을 변경하여 서비스 ID를 업데이트할 수 있습니다. 또한 필요에 따라 키를 삭제하고 새 API 키를 작성하거나 지정된 액세스 정책을 업데이트할 수도 있습니다. 하지만 기존 서비스 ID를 변경하면(예: 지정된 정책 변경 또는 현재 사용 중인 API 키 삭제) 이 서비스 ID를 사용하는 애플리케이션에서 서비스가 중단될 수 있습니다.

## 서비스 ID 사용 방법에 대한 예제

다음은 {{site.data.keyword.objectstorageshort}} 및 Cloud SQL Query 서비스에 서비스 ID를 사용하는 방법에 대한 예제입니다.

- {{site.data.keyword.objectstorageshort}} - [시작하기](/docs/services/cloud-object-storage/getting-started-cli.html#getting-started-cli-).
- Cloud SQL Query - [SQL Query REST API 사용 방법 ![외부 링크 아이콘](../icons/launch-glyph.svg)](https://www.youtube.com/embed/s6S4AdJItHk?rel=0){: new_window}.
