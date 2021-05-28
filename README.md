# React-Native Navigation
## Getting started 
- Installation
```
npm install @react-navigation/native
```
- Installing dependencies into a bare React Native project
```
npm install react-native-reanimated react-native-gesture-handler react-native-screens react-native-safe-area-context @react-native-community/masked-view
```
-------------------------
## Hello React Navigation
- Installing the stack navigator library
```
npm install @react-navigation/stack
```

## Moving between screens
- 웹 브라우저의 경우 아래와 같이 href 속성이나 onClick 이벤트를 사용한다.
```html
<a href="details.html">Go to Details</a>
```
혹은
```html
<a
  onClick={() => {
    window.location.href = 'details.html';
  }}
>
  Go to Details
</a>
```

- 리액트 네이티브에서는 onPress()를 이용한다.
```javascript
import * as React from 'react';
import { Button, View, Text } from 'react-native';  // 사용하는 컴포넌트 임포트!!!
import { NavigationContainer } from '@react-navigation/native';  // add
import { createStackNavigator } from '@react-navigation/stack';  // add

function HomeScreen({ navigation }) {
  return (
    <View style={{ flex: 1, alignItems: 'center', justifyContent: 'center' }}>
      <Text>Home Screen</Text>
      <Button
        title="Go to Details"
        onPress={() => navigation.navigate('Details')}
      />
    </View>
  );
}
```

- navigate() -> push() 사용
```javascript
onPress={() => navigation.navigate('Details')  // Details페이지에서 버튼을 클릭해도 아무 변화 없음
onPress={() => navigation.push('Details')  // Details페이지에서 버튼을 클릭하면 Details페이지가 계속 쌓임
```

## Tab navigation
- Install
```
npm install @react-navigation/bottom-tabs
```

## Drawer navigation
- Install
```
npm install @react-navigation/drawer
<<<<<<< HEAD
```
=======
```
>>>>>>> 5d699660a5dc3818cb7c03979d26b353b4bf86c9
