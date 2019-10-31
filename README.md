# react_Navigation

Bismillahirahmanirrahim...
---------------------------------------
: npm install --save react-navigation :
---------------------------------------
//untuk bagian App.js\\

import React, {} from 'react';
import {} from 'react-native';
import {createStackNavigator, createAppContainer} from 'react-navigation';
import Home from './components/HomeScreen';
import Setting from './components/Setting';

const AppNavigator = createStackNavigator({
  HomeScreen:{
    screen:Home,
    navigationOptions:{
      hender:null
    }
  },
    SettingScreen:{
    screen:Setting,
    navigationOptions:{
      hender:null
    }
  },
});
export default createAppContainer(AppNavigator);
__________________________________________________________________________________________________________________ !
//untuk bagian HomeScreen.js\\

import React, {Component} from 'react'
import {View, Text, Button} from 'react-native'

export class Setting extends Component{
  render(){
    return(
      <View>
      <Text>selamat datang</Text>
        <Button 
        title='HOME'
        onPress={()=>this.props.navigation.navigate('SettingScreen')}/>
      </View>
    )
  }
}
export default Setting;
__________________________________________________________________________________________________________________ !
//untuk bagian SettingScreen.js
import React, {Component} from 'react'
import {Text, View} from 'react-native';

export default class HomeScreen extends React.Component{
  render() {
    return(
      <View>
      <Text>Selamat Tinggal</Text>
      </View>
    )
  }
}

Semoga Bermanfaat
