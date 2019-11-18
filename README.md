<div align="center">
  <h1>
    <br/>
    <br/>
    ️📝
    <br />
    <br />
    WIL : What I want to Learn
    <br />
    <br />
    <br />
    <br />
  </h1>
  <sup>
    <br />
    <br />
    <br />
    공부할 거리, 만들 거리.
    <br />
    <br/>
    
   RealTime To-Do : [👻](https://github.com/purelledhand?tab=projects)
    
  </sup>
  <br />
  <br />
  <!--pre>cd demo<br/>yarn start</pre-->
  <br />
</div>
<div>
<h4>filesystem</h4>
  <sup>
wen-xu, file  system fuzzing 논문 리딩
  <br />
    TSK, Hikvision
  <br />
    Facebook, find a needle in the haystack 논문 리딩 (엄밀히 나누면 Filesystem이라기 보단 Storage Architecture)
  <br />
    Google, GFS 논문 리딩
  <br />
  </sup>
  <h4>Project Scaffolding</h4>
  <sup>
  Gymana : FE Project Scaffolding 정리
  <br />
  UnifoCS : Project Scaffolding 정리
  <br />
  </sup>
  <h4>Web System Engineering</h4>
  <sup>
REST API 논문 리딩
  <br />
    JEST로 react unit test 코드 작성하기
  <br />
    https://github.com/larrybotha/testing-javascript
    <br />
    11/11일에 느낀 MVC, MVVP, FLUX 패턴 vue/react 관점에서 생각난거 정리하기 (model - view 사이에서 바인딩이 발생할때의 문제점 등)
  <br />
    가벼운 토이프로젝트 Redux, Mobx로 마이그레이션하면서 상태관리 해보기
  <br />
    가벼운 토이프로젝트 Context API로 anti-redux하기
  <br />
    SCE338 Project FE Scaffold 정리
    <br />
    재현이랑 DB 트랜잭션 원리 정리
    <br />
    Dan Abramov의 리액트 라이브 : Hot Reloading으로 시간 여행 떠나기 :  https://www.youtube.com/watch?v=xsSnOQynTHs
    <br />
    Virtual DOM, DOM and Render in Browsers 과정 정리
    <br />
    Dalvic, ART 비교하면서 유저가 설치하는 시간은 오래걸려도 신경쓰지않는다고 했던 거랑 클라이언트 렌더링이랑 엮은 글 쓰기
  <br />
    자동으로 Rest API Document 만들어주는 서비스
  <br />
    https://yesno.wtf/api 사용해서 결정장애왔을때 바로 답받아서 카톡으로 보내주는 서비스 (IFTTT?)
    <br/>
    스타벅스에서 호감있는 여성끼리 친해질 수 있는 서비스.. (내 앞에 여성분 나랑 굿즈취향도 잘맞고, 키보드랑 스탠드 세팅해서 일하는 모습 너무 멋지당.. 친해지고 싶당..)
  <br />
    
   [Discord가 React-Native로 iOS에서 Native 수준의 퍼포먼스를 낸 방법](https://blog.discordapp.com/how-discord-achieves-native-ios-performance-with-react-native-390c84dcd502) : 크롬 프로파일러와 React 프로파일러를 이용해서 느린 부분을 찾고 해결한 방법들 정리
    
  </sup>
  <h4>Devops</h4>
  <sup>
orchestration - Swarm으로 vhost할 때 레이어링 이슈랑 Kube custom으로 해결할 수 있는 부분 포스팅하기
  <br />
    S3에 파일 올릴때마다 Cloudfront 캐시 무효화하는 람다 스크립트 완성하기
  <br />
    개인 페이지 serverless architecture : Fauna + AWS lambda + netlify (토폴로지 그려놓기)
  <br />
    고민 : Fauna DB -> DB 비용 X, 다른 리전일 경우 네트워크 트래픽 비용이 발생할 수 있음 / RDS -> 네트워크 비용X, DB 비용O / 두 경우 비용 비교하기
  <br />
    https://github.com/netlify/netlify-faunadb-example
  <br />
    https://github.com/serverless/examples/tree/master/aws-node-graphql-api-with-dynamodb
    <br />
    https://serverless.com/learn/courses/serverless-for-frontend-developers/
    <br />
    event-driven concept
    <br />
  </sup>
  <h4>Android</h4>
  <sup>
nmap으로 포트 별 서비스 버전 스캔 후 서비스 버전 별 CVE 알려주는 앱 개발
  <br />
  </sup>
    <h4>V8</h4>
  <sup>
<br />
  
[JavaScript 엔진 톺아보기(1)](https://velog.io/@godori/JavaScript-engine-1)
  
[자바스크립트는 어떻게 작동하는가: V8 엔진의 내부 + 최적화된 코드를 작성을 위한 다섯 가지 팁](https://engineering.huiseoul.com/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8%EB%8A%94-%EC%96%B4%EB%96%BB%EA%B2%8C-%EC%9E%91%EB%8F%99%ED%95%98%EB%8A%94%EA%B0%80-v8-%EC%97%94%EC%A7%84%EC%9D%98-%EB%82%B4%EB%B6%80-%EC%B5%9C%EC%A0%81%ED%99%94%EB%90%9C-%EC%BD%94%EB%93%9C%EB%A5%BC-%EC%9E%91%EC%84%B1%EC%9D%84-%EC%9C%84%ED%95%9C-%EB%8B%A4%EC%84%AF-%EA%B0%80%EC%A7%80-%ED%8C%81-6c6f9832c1d9)

  v8 터보팬
  <br />
    v8 인터널 (빌드 다들 어느정도 걸리는지 물어보기)
  <br />
  </sup>
  
</div>
