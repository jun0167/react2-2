# 이준희 202030228

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