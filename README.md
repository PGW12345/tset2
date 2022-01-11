# tset2
T2

import {NavigationContainer} from '@react-navigation/native';
import {createStackNavigator} from '@react-navigation/stack';
import React from 'react';
import Main from './screens/Main';
import Home from './list/Home';

const Stack = createStackNavigator();

const App = () => {
  return (
    <NavigationContainer independent={true} initialRouteName="Main">
      <Stack.Navigator screenOptions={{headerShown: false}}>
        <Stack.Screen name="Main" component={Main} />
        <Stack.Screen name="Home" component={Home} />
      </Stack.Navigator>
    </NavigationContainer>
  );
};

export default App;
