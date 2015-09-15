---
title: Step 6: 새로운 콘텐츠를 작성하기
lang: ko
summary: '이것은 편집자 가이드 Step6 입니다..'
tags:
  - Basic
  - Pages
uri: 'WPD:Editors Guide/step 6 author or upload new content/ko'

---
## <span>Summary</span>

이것은 편집자 가이드 Step6 입니다..

## <span>Step 6. 새로운 콘텐츠를 작성하기</span>

### <span>새로 작성한 콘텐츠가 사이트에 적합한지 확인하기</span>

-   토픽이 이미 존재하는지 확인하기 위해 [고급 검색 페이지](http://docs.webplatform.org/w/index.php?title=Special:Search)를 사용하세요.
-   WebPlatform.org의 목표를 배우고 WebPlatform.org를 관장하는 세가지 pillars를 확인하기 위해 [Pillars page](/WPD:Policy/Pillars)를 참조하세요.

### <span>여러분이 새로운 콘텐트를 추가하는 것을 팀에게 알려주세요.</span>

-   온라인 상에서 문의하는 방법을 확인하기 위해 [편집자 가이드 Step 2](/WPD:Editors_Guide/step_2_communicate_with_the_online_community/ko)를 확인하세요.

### <span>새로운 콘텐츠를 준비하기</span>

-   코드 스니핏에 적절한 구문 highlighting을 적용하고 위키 문법을 사용하는 페이지를 만드는 방법을 배우기 위해 [편집자 가이드 Step 5](/WPD:Editors_Guide/step_5_update_existing_content/ko)를 참고하세요.
-   [Yahoo 스타일 가이드](http://styleguide.yahoo.com/)의 컨벤션을 따르세요.

### <span>위키에서 새 페이지 만들기</span>

-   대부분의 경우에 여러분은 [New Page page](/WPD:New_Page)의 form을 사용할 수 있습니다.
-   여러분이 튜토리얼과 컨셉트 글을 작성하는 경우 [튜토리얼과 컨셉트 글 페이지](/WPD:Content/Tutorials_and_concept_articles)를 따르세요.
-   여러분이 참조 문서를 작성하는 경우 [참조 글 페이지](/WPD:Content/Reference_articles)를 확인 하세요.
-   여러분이 API 문서를 작성하는 경우 [API 문서 페이지 만들기](/WPD:Creating_API_pages)를 읽어 주세요.

### <span>새 페이지를 만들 위치를 선택하기</span>

-   위키 안의 페이지를 구조화하는 방법을 배우려면 [Topic hierarchy page](/WPD:Content/Topic_Hierarchy)를 확인해 주세요.
-   여러분이 만드는 새 페이지를 저장하기 위한 위치를 선택하기 위해 [Architecture page](/WPD:Architecture)를 확인해 주세요.
-   새 페이지를 만들기 위한 섹션이 확실치 않다면 지침에 대해 문의 하는 방법을 배우기 위해 [편집자 가이드 Step 2](/WPD:Editors_Guide/step_2_communicate_with_the_online_community/ko)를 확인해 주세요.

### <span>새 페이지에 대한 유효한 URL 만들기</span>

다음으로 [New Page page](/WPD:New_Page)로 이동하여 정의된 콘텐츠 페이지 템플릿 중 하나를 사용하여 새 페이지를 만들어 주세요. 여러분이 페이지를 만들때 여러분이 path 텍스트 박스에 입력한 텍스트가 새 패이지의 URL이 된다는 것을 기억해 주세요. 또한 페이지 URL은 페이지 제목으로 보여지는 것과 일치할 필요가 없다는 것을 숙지하세요.

예를 들면 "eventsource\_basics" 이라는 URL을 갖는 페이지는 "Streaming updates with server-sent events"이라고 내부적으로 제목을 가질수 있습니다. 목표는 URL을 짥고, 충분히 설명되며, 유일한 값으로 유지하는 것입니다.

-   올바른 문법을 위해 절대적인 경우를 제외하고 URL안의 문자는 대문자를 쓰지 않습니다. 예를 들어 여러분이 user media에 관한 글을 작성한다면 여러분은 getUserMedia 메서드에 관한 글의 경우 getUserMedia라고 입력하는 대신에 usermedia라고 입력 할수 있습니다.
-   underscore는 페이지가 만들어질때 space의 위치에 자동적으로 생성되기 때문에 URL에서 분리된 단어들을 표현하기 위해 underscore 대신 space를 사용하세요. 예를 들어 여러분이 HTML5 audio tag에 관한 새 글을 만든다면 여러분은 audio tag라고 입력 할수 있으며 생성된 URL은 audio\_tag가 될 것입니다.
-   URL 안에 대시 또는 괄호와 같은 다른 구두점을 사용하지 마세요. URL안에 구두점을 추가하는 것은 주요 사이트의 문제들을 일으키기 때문에 특별히 중요합니다.
-   절대적으로 필요한 경우가 아니라면 URL 안에 the, a, an을 사용하지 마세요.

### <span>깨진 링크를 확인하세요.</span>

-   기존 페이지를 이동하기 전에 [기존 문서에 대한 링크를 포함하고 있는 페이지](http://docs.webplatform.org/w/index.php?title=Special%3AWhatLinksHere&target=Template%3ACompat+Unknown&namespace)를 식별하고 여러분이 생성한 새로운 URL을 사용하기 위해 이 페이지들의 링크를 업데이트 하세요.

### <span>크로스 브라우서 호환성을 위한 기능을 확인 하세요.</span>

호환성 표는 CSS, HTML, JavaScript 기능, API들이 어느 브라우저에서 지원되는지, 브라우저 버전에 따라 지원여부에 대한 상세 정보를 제공하세요. 이 표는 헤더(데스크탐과 모바일을 위한 분리된 호환성 섹션)와 함께 템플릿안에 포함되어야 합니다. 아래는 호환성표의 스크린 샷입니다.

![Screenshot of a compatibility table.](/WPD/assets/public/7/73/compatibility_table.png)

표는 [호환성 정보를 잃어버린 페이지들의 동적인 목록](http://docs.webplatform.org/w/index.php?title=Special%3AWhatLinksHere&target=Template%3ACompat+Unknown&namespace=)에 나타남에 따라 자동적으로 플래그가 지정됩니다.

 이 사이트의 목적을 위해 모던 브라우저에서의 기술지원 여부가 가장 중요합니다. 만약 어떤 프로퍼티가 IE 4 또는 Safari 1에서 지원되다면 그것은 가장 최근 브라우저 버전에서의 호환성 여부를 알리는 것보다 중요하지 않습니다.

각각의 항목에 대해여 브라우저 버전에 대해 완벽히 지원되는지 우선 확인하세요. 만약 부분적인 지원으로만 현재 제공된다면 버전 번호 뒤에 단어(부분)을 추가하여 명시해 주세요.

-   각 브라우저에서 지원되는 각 기술들을 배우기 위해 다음의 상호 호환 온라인 리소스를 확인하세요
-   [www.caniuse.com](http://caniuse.com/)
-   [Compatibility section on www.quirksmode.org](http://www.quirksmode.org/compatibility.html)
-   [Mozilla Developer Network site](http://developer.mozilla.org)

Mozilla Developer Network는 기여자들이 저작권 표시 없이 기본적인 사실들(브라우저 버전 번호, 지원에 대한 yes/no/partial 정보)에 대해 복사하는 것을 허락하는 것에 대해 동의했습니다. 다른 온라인 상의 리소스들에서 연구되는 호환성 사실들은 [저작권 표시 지침](http://docs.webplatform.org/wiki/WPD:External_Attribution)에 따라 확인해 주세요.

각각의 element가 지원되거나 그렇지 않은 경우(라디오 버튼을 yes,no,unknown으로 선택함에 따라)를 명시합니다. 만약 항목이 지원되는 경우 그것을 지원하는 브라우저의 최소 버전을 명시합니다.(그리고 모든 더 높은 버전들은 그것을 지원한다고 가정합니다.)

몇몇 element에 대해 개별적으로 호출되는 것이 필요한 sub-element 또는 기능들이 있을수 있습니다. 이것들은 여러분이 Basic Support에 대해 다룬 후에 여러분이 표에 부가적인 행들을 추가하기 위해 "Add Another"버튼을 클릭할수 있습니다.

여러 행 호환성 정보 표의 예제를 보려면 브라우저간 큰 차이로 지원되고 있으며 HTML5 규격안에서 다뤄지는 다양한 오디오 코덱들을 위하여 분리된 행들을 포함하고 있는 [Audio tag](http://docs.webplatform.org/w/index.php?title=html/elements/audio)를 확인하세요.

부가적인 행들은 이름으로 정렬되어야 합니다. 표에서 항목을 위 혹은 아래로 움직이기 위해 "Remove" 버튼의 오른 쪽의 handle을 드래그하여 사용합니다.

Compatibility Notes를 위한 부분은 호환성 섹션안의 세번째 표입니다. 이것은 단지 yes/no 그리고 버전넘버를 명시하는 것으로 다룰수 없는 것들을 다루기 위해 사용합니다.

### <span>토픽과 토픽 클러스터</span>

일반적으로 우리는 글의 가장 낮은 레벨의 단위(글에 대한 것)에서 글을 설명하기 위해 토픽을 사용합니다. 글은 하나 이상의 토픽을 가질 수도 있습니다. 우리는 유사 토픽들의 글을 그룹화하여 토픽 클러스터로 사용합니다. 토픽 클러스터는 See Also 섹션에서 관련된 토픽들의 목록을 만들어 냅니다. 다음 섹션은 토픽과 토픽 클러스터의 사용 예에 대해 설명합니다.

### <span>토픽 사용 예</span>

다음 목적들로 글을 설명하기 위해 토픽들을 사용하세요. 이 사용 예들은 상호배제적이 아니며 여러분은 하나 혹은 둘다 사용할수 있음을 숙지하세요.

#### <span>기본 메타 데이터</span>

토픽들은 키워드로 글의 콘텐츠를 설명합니다. "usefully"를 적용할 만큼 표시 합니다. 너무 많은 메타 데이터는 그림을 흐릴수 있어 너무 적은 것보다 나쁩니다. 토픽 키워드는 검색엔진 최적화와 콘텐츠 분류체계를 효과적으로 설명하는 것과 같은 몇가지 용도를 가집니다. 이 분류체계는 여러 측면이 있습니다. 예를 들어 CSS-Regions API는 API(컨텐츠의 목적)이며 CSS에 대한 것(컨텐츠의 주제)입니다. 또한 그것은 CSS-Regions에 대해 구체적입니다. 그러나 CSS-Regions 토픽 태그는 일반적인 메타 데이터보다 더 구조와 탐색을 묘사하기 위해 특화되어 사용됩니다. 다음을 보세요.

#### <span>API 기본 목록 구성 검색어</span>

글의 템플릿 타입의 문맥 안에서 글을 설명하기 위해 토픽을 사용하세요.(이것은 [WPD:New\_Page](/WPD:New_Page) 페이지에서 설명하고 있습니다.) 즉, 페이지가 어떤 API 오브젝트(API\_Object 템플릿으로 사용됩니다.)를 위한 것이고 그 글은 CSS-Regions API에 대한 것이라면, 토픽 체크박스는 "CSS-Regions"에 체크되어야 합니다. 이것은 여러분이 모든 API 오브젝트 요약 표에서 생산된 API\_Listing 페이지 안에서 "[[Category:CSS-Regions]][[Category:API\_Objects]]"와 같은 검색어로 지정하는 것을 가능하게 합니다. 이 검색어가 얘기하는 것은 "CSS-Regions 토픽의 페이지들(API\_Object 페이지들도)을 나에게 읽어와라"입니다. 이것은 모든 API에 토픽이 지정되어야 함을 의미합니다.

검색어는 일반적인 Category:CSS 이상을 선택하지 않는 것을 주의 하세요. 만약 다른 CSS 관련 Javascript API들이이 있다면, 즉 CSS-Overlay(이것은 가정입니다.)가 있다면, 만약 Category:CSS에 대한 검색 결과가 CSS-Regions와 CSS-Overlay API\_Listing 페이지들이라면 두 API들의 모든 오브젝트들이 각각의 API의 요약 표에 나타날 것입니다. 중복이 발생하는 것을 막는 방법은 하나의 API\_Listing 안의 모든 API\_Object 페이지에 대하여 구별된 토픽을 만드는 것입니다.

더 많은 정보는 [API 페이지 만들기](/WPD:Creating_API_pages#Object_listing_page_content)를 참고하세요. 새 토픽들을 만드는 방법은 [WPD:Topics](/WPD:Topics)를 참고하세요.

### <span>토픽 클러스터 사용 예</span>

See Also 섹션에서 관련 콘텐트 글 목록을 생성하는 것은 토픽 클러스터를 사용하세요. 위키-튜토리얼들, 컨셉트들, API들, HTML element들 등과 같은 많은 도메인을 가로질러 글을 가져오기 위한 방법이 여기 있습니다. 때때로 이 글들은 "WebRTC"와 같은 공통 용어를 공유하게 됩니다. 그러나 때때로 공통 용어가 불명확 해지기도 합니다.

[apis/navigation\_timing](/apis/navigation_timing), [apis/resource\_timing](/apis/resource_timing), [apis/user\_timing](/apis/user_timing)와 같은 세가지 Timing API들로 예를 들면 여러분은 이것들이 "Timing" 토픽 클러스터를 공유하고 있다고 생각할 수 있습니다. 그러나 그렇게 되면 여러분의 토픽 클러스터는 최적화, 디버깅, 성능 관련 글 모두를 놓치게 됩니다. 아마도 이 경우에서 최적의 토픽 클러스터는 "Performance"일 것입니다.

**Careful!** 똑같은 토픽 클러스터로 너무 많은 글을 태깅함으로서 토픽 클러스터를 남용하기 쉽습니다. 불필요한 링크들의 긴 목록을 만들게 됩니다. 예를 들면 API 오브젝트 멤버들(이벤트들, 메소드들, 그리고 프로퍼티들)은 토픽 클러스터가 될 필요가 없으며 오로지 API 오브젝트가 토픽 클러스터가 될 필요가 있습니다. 또한 "CSS"와 같은 큰 범위의 토픽 클러스터를 사용하는 것을 피해야 합니다. 다시 말하면 여러분은 관계없는 항목들의 큰 목록을 얻게 될 것 입니다.

새로운 토픽 클러스터를 만들려면 [Property:Topic\_Cluster](/Property:Topic_Cluster)의 리스트에 그것을 추가하세요.

### <span>호환성 상태 업데이트</span>

만약 여러분이 페이지의 호환성 표를 완료했다면(데스크탑과 모바일 브라우저 모두에 대해), 여러분은 영어버전에서 글의 왼쪽에 있는 페이지 제목 바로 아래 콘텐츠 섹션에서 호환성 관련 완료되지 않은 체크박스를 선택하지 않을 수 있습니다.

여러분이 수정하거나 저작하고 있는 페이지이며 호환성 정보가 필요하지 않다고 느껴졌다면 (그리고 현재 [페이지가 누락된 호환성 정보와 함께 페이지로 표시됩니다.](http://docs.webplatform.org/w/index.php?title=Special%3AWhatLinksHere&target=Template%3ACompat+Unknown&namespace=)) 여러분은 이 섹션이 필요하지 않다고 지시하는 호환성 섹션 헤더 아래의 체크박스를 즉시 체크할수 있습니다.(그리고 사이트 상에 나타나지 않는지 확인해 주세요.) 또한 위에서 설명한대로 페이지의 상단 근처의 Compatibility Incomplete 체크박스 선택도 취소해야 합니다.

여러분의 마지막 요약(커밋) 의견은 여러분이 호환성 정보의 상태를 변경했는지 언급해야 합니다.

### <span>이미지 링크 또는 다른 리소스(assets)를 페이지에 업로드 하기</span>

이미지 파일들과 다른 리소스(assets)를 준비하고 업로드 하는 방법을 배우기 위해 [편집자 가이드 Step 7](/WPD:Editors_Guide/step_7_prepare_and_upload_assets_for_articles)을 참고하세요. 파일은 한번 업로드 되면 그것에 대한 링크를 추가할 수 있습니다.

### <span>여러분의 작업물을 저장하세요.</span>

페이지 상에서 여러분의 수정이 완료된 후에 요약 필드안에 여러분의 변경사항들의 요약을 입력합니다. 여러분이 단지 기존 정보를 약간 조정하였다면 minor edit 체크박스에 체크합니다. 여러분의 작업을 확인하기 위해 (추천되는 작업입니다.) 프리뷰 보기 버튼을 클릭합니다. 그리고 여러분의 변경사항을 저장하기 위해 페이지 저장하기 버튼을 클릭합니다.

**Note**: 만약 여러분이 저장없이 잠시동안 편집한 경우 여러분의 세션 정보가 오래되어 다음과 같은 경고 메시지를 받을 수 있습니다:

**Sorry! We could not process your edit due to a loss of session data. Please try again....** ""죄송합니다! 우리는 세션 데이터가 없어져 편집을 처리할 수 없습니다. 다시 시도해 주세요..."" (여러분의 처리되지 않은 새버전의 프리뷰와 수정된 소스와 함께...)

여러분이 이 에러를 받으면 페이지 저장하기 버튼을 다시 클릭하세요. 대부분의 경우 단순한 resubmitting으로 form은 동작할 것 입니다. (첫번째 시도에서 여러분의 세션이 갱신되었디 때문에 두번째 시도에서 제출이 가능해 집니다.)

### <span>예외 추가</span>

만약 여러분이 어떤 외부 이슈들, 페이지에 관한 항목들 혹은 질문들을 언급하기 원한다면 메시지와 함께 페이지 상에 다음 태그를 추가해 주세요:

{{TODO | [이것은 이 페이지에서 여전히 누락된 항목들의 설명입니다.] }}

### <span>템플릿 작업 방법에 대한 부가적인 정보 얻기</span>

이 위키는 규격화와 표준화된 페이지 컨텐츠를 위해 템플릿을 사용합니다. 이 기여를 위해 필요하지 않지만 여러분은 위키 장면 뒤의 작동 방법에 대한 세부사항을 얻을 수 있습니다.

-   여러분이 템플릿이 작동하는 방법을 탐구하려는 경우 [패턴 페이지 구현](/WPD:Implementation_Patterns)을 확인해 주세요.

