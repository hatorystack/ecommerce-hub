---
id: introduction
sidebar_position: 4
displayed_sidebar: shopifySidebar
slug: /shopify/theme/liquid
tag: shopify
---

# 소개

## Liquid
Liquid는 쇼피파이에서 동적인 콘텐츠를 효율적으로 관리하기 위해 오픈 소스 형태로 공개한 템플릿 언어입니다. 쇼피파이에서 사용되고 있는 모든 스토어 디자인 테마를 포함, 다양한 소프트웨어 프로젝트에서 사용되고 있습니다.

## 템플릿 언어
템플릿 언어란 정적인 요소들을 재사용할 수 있는 레이아웃을 정의하고 동적인 콘텐츠들을 표시하기 위해 사용합니다.
(예: 정적 HTML 페이지 안에서 Liquid 문법을 사용하여 동적인 콘텐츠 표시)

## Liquid 구문
Liquid는 `objects`, `tags`, `filters` 들을 조합하여 동적인 콘텐츠를 표시합니다. HTML 문법과 구분하기 위해서 `{{ }}`, `{% %}` 같은 구획 문자를 제공합니다.

> ### Objects
> Objects는 페이지에 표시될 출력 데이터로, 템플릿에서 이중 중괄호 `{{ }}`로 감싸 표시합니다.
> ```
> Input: {{ shop.name }}
> Output: "스토어 이름"
> ```
> ### Tags
> Tags는 템플릿에서 논리적인 제어의 흐름을 만들기 위해 사용합니다. 중괄호와 백분율 기호로 감싼 영역에 사용할 제어 구문을 입력하여 설정합니다.  템플릿 렌더링 시 입력된 제어 구문은 화면에 표시되지 않은 체 해당 제어 구문만 실행됩니다. 변수 할당, 조건문, 반복문 로직을 화면에 표시하지 않고 사용할 수 있습니다.
> ### Filters
> ```
> Input: 
>   {% if product.available %}
>      가격: $99.99
>   {% else %}
>      죄송합니다. 해당 상품은 품절되었습니다.
>   {% endif %}
> Output: "가격: $99.99"
> ```