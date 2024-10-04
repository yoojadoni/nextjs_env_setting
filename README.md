# nextjs_env_setting
nextjs에서 env 설정

nextjs 14.2.3 기준 으로 
env cmd 설치후 
1. script 생성
   package.json 파일에서 아래 참고 작성
"scripts"{
  "dev" : "next dev",
  "build:dev" : "env-cmd -f .env.dev next build",  
  "build:local" : "env-cmd -f .env.local next build",
  "build:q" : "env-cmd -f .env.q next build",
  "build:live" : "env-cmd -f .env.live next build",
}

2. env파일 생성
.env.서버타입(local, dev, q, live) 파일 생성 

3. 빌드 방법 
npm run build:live
npm run build:local
npm run build:dev
npm run build:q

