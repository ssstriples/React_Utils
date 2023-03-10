# React

## React Util 제작 
1. Parsing/Making TLV Packet
2. Parsing/Making CV Packet
4. Parsing/Making FID Packet(에솔에선 device info:0x31 주로 확인 필요)
5. Simulator(AwsIoT -> **Cloudlet** <- Common)
6. Service Server APIs
    - login for emp-token
    - modelTypes
7. ETC
    - manufacture injection for QR Registration

### 1. 개발 환경 설정
- yarn 설치
```
npm install --global yarn
yarn --version
```

- 프로젝트 생성(todo-app 예제)
```
yarn create react-app todo-app
```

#### 1-1. Prettier설정
- 프로젝트 최상위 디렉터리에 .prettierrc 파일 생성
```javascript
{
    "singleQuote": true,
    "semi": true,
    "useTabs": false,
    "tabWidth": 4,
    "trailingComma": "all",
    "printWidth": 80
}
```

#### 1-2. index.css 수정
- 프로젝트의 글로벌 스타일 파일 index.css 수정
```css
body {
    margin : 0;
    padding : 0;
    background : #e9ecef;
}
```

#### 1-3. App 컴포넌트 초기화
```javascript
const App = () => {
  return <div>Todo App</div>
};

export default App;
```

### 2. UI구성

#### 2-1.