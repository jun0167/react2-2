# 이준희 202030228

## 9월 11일 강의

#### SSG ####
###### [SSG 주요 이점] ######
- **쉬운 확장** -- CDN을 통해 파일 제공, 캐쉬에 저장
- **뛰어난 성능**  -- 클라이언트나 서버가 무언가를 처리할 필요 X
- **더 안전한 API 요청** -- 외부 API 호출, 데이터베이스 접근 보호해야 할 데이터에 접근 할 일 X   
필요한 모든 정보가 빌드 시점에 미리 페이지로 렌더링 되어있음 

#### CSR ####  


###### [CSR 주요 이점] ######  
- 네이티브 앱처럼 느껴지는 웹 앱  
- 쉬운 페이지 전환 
▶ **장점은 단점이 될 수도 있습니다.** 
- 네트워크 속도가 느린 환경에서는 번들이 모두 다운로드 될 때까지 계속 빈 페이지를 보아야 합니다.  
- 검색 로봇에게도 그 내용은 빈 것으로 보입니다.  
- 번들을 모두 받을때 까지 검색 로봇이 기다리기는 하지만 성능 점수는 낮을 것입니다. 


#### 서버 사이드 렌더링(SSR) ####
▼ 렌더링 전략
- 렌더링 전략이란? 웹 페이지 또는 웹 애플리케이션을 웹 브라우저에게 제공하는 방법  
- 정적인 페이지 제작에는 Gatsby  
- 서버 사이드 렌더링 전략을 원한다면 다른 프레임워크 검토  
- Next.js 에서는 이 모든 방법을 완전히 새로운 수준으로 제공  
- 어떤 페이지는 빌드 시점에 정적으로 생성,   
  어떤 페이지는 실행 시점에 동적으로 생성


###### [SSR의 장점] ######  
- **더 안전한 웹 애플리케이션**: 쿠키 관리 , 주요 API, 데이터 검증 등과 같은 작업을 서버에서 처리하기 때문에 중요한 데이터를 클라이언트에 노출할 필요가 없기 때문입니다.  
- **더 뛰어난 웹 사이트 호환성**: 클라이언트 환경이 자바스크립트를 사용하지 못하거나 오래된 브라우저를 사용하더라도 서비스를 제공할 수 있습니다.  
- **더 뛰어난 SEO** : 서버가 랜더링한 HTML을 받기 때문에 봇이나 웹 크롤러가 페이지를 렌더링할 필요가 없기 때문입니다.

###### [SSR이 최적의 렌더링 전략이 아닌 경우] ######  
- 클라이언트가 페이지를 요청할 때마다 페이지를 다시 렌더링할 수 있는 서버가 필요합니다.  
- 다른 방식에 비해 SSR이 더 많은 자원을 소모하고, 더 많은 부하를 보이며 유지 보수 비용도 증가합니다.  
- 페이지에 대한 요청을 처리하는 시간이 길어집니다.  
  

## 9월 4일 강의

#### 프로젝트 기본 구조 ####
* Next.js 는 네비게이션을 구현할 때 react-router와 같은 라이브러리를 사용하지 않고,  
 pages/디렉토리를 사용합니다.  
#### 프로젝트 생성 방법 ####
* create-next-app 을 이용하여 프로젝트 생성.  
##### nvm 사용법 ▼ #####

  * nvm arch                     : Show if node is running in 32 or 64 bit mode.
  * nvm current                  : Display active version.  
  * nvm debug                    : Check the NVM4W process for known problems (troubleshooter).    
  * nvm install <version> [arch] : The version can be a specific version, "latest" for the latest current version, or "lts" for the
                                 most recent LTS version.  
  * nvm list [available]         : List the node.js installations. Type "available" at the end to see what can be installed. Aliased as ls.  
  * nvm on                       : Enable node.js version management.  
  * nvm off                      : Disable node.js version management.  
  * nvm proxy [url]              : Set a proxy to use for downloads. Leave [url] blank to see the current proxy.       
  * nvm node_mirror [url]        : Set the node mirror. Defaults to https://nodejs.org/dist/. Leave [url] blank to use default url.  
  * nvm npm_mirror [url]         : Set the npm mirror. Defaults to https://github.com/npm/cli/archive/. Leave [url] blank to default url.  
  * nvm uninstall <version>      : The version must be a specific version.  
  * nvm use [version] [arch]     : Switch to use the specified version. Optionally use "latest", "lts", or "newest".     
  * nvm root [path]              : Set the directory where nvm should store different versions of node.js.
  * nvm [--]version              : Displays the current running version of nvm for Windows. Aliased as v.