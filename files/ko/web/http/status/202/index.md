---
title: 202 Accepted
slug: Web/HTTP/Status/202
tags:
  - HTTP
  - Reference
  - Status code
translation_of: Web/HTTP/Status/202
---
{{HTTPSidebar}}

HTTP **`202 Accepted`** 는 요청이 성공적으로 접수되었으나, 아직 해당 요청에 대해 처리 중이거나 처리 시작 전임을 의미합니다. 요청이 처리 중 실패할 수도 있기 때문에 요청은 실행될 수도 실행되지 않을수도 있습니다.

이 상태 코드는 비확약적, 즉 HTTP가 나중에 요청 처리 결과를 나타내는 비동기 응답을 보낼 방법이 없다는 것을 의미합니다. 이는 다른 프로세스나 서버가 요청을 처리하는 경우 또는 일괄 처리를 위한 것입니다.

## 상태

```
202 Accepted
```

## 명세

{{Specifications}}

## 같이 보기

- {{HTTPHeader("Accept")}}
