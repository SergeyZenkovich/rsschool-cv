# Sergey Zenkovich

## Contact Info:
* Telegram  - https://t.me/SergeyZenkovich
* Mobile - +375(29)8868275 
* E-mail - sapocalipsys.z@gmail.com
* Skype - sergeyilsk
* LinkedIn - https://www.linkedin.com/in/sergey-zenkovich-2a0a72183

## Summary:
 I am reseacher in GIS and remote sensing areas. In 2019 I graduated from the University(BSU - geography faculty - GIS specialist). Now I am working with spatial data, analyzing space images, writing scripts for GIS software environment. For me it's interesting to try out FrontEnd. I have some experience in FrontEnd (completed courses: “FrontEnd start” in TeachMeSkills, try out: “RSSchool-2019/2020”). My goal is to improve my hard skills in FrontEnd and interconnect my knowledges of GIS and spatial data analyzing and FrontEnd in my future job.<br/> 
**Goal** - Work as a Front-End developer in a big product company. <br/>

**Wishes:**
 * Impove my hard sklls.
 * Work with AR, VR technologies and 3d visualization.
 * Try myself in web design. 

## Hard skills:
* HTML5 + semantic HTML
* CSS3 + Sass + Less
* Bootstrap
* ES 5 + ES next
* JQuery
* React
* Redux
* Material UI
* Git
* Webpack
* Phyton 
* SQL
* BEM methodology
* Responsive design

## Code examples:
```Javascript
	function swapHeadAndTail(arr) {
		const even = arr.length % 2 === 0;
		if (even) {
		 	 const firstHalf = arr.filter((elem, index) => index < arr.length / 2);
		 	 const secondHalf = arr.filter((elem, index) => index >= arr.length / 2);
		 	 return […secondHalf, …firstHalf]; 
		}
		const firstHalf = arr.filter((elem, index) => index < arr.length / 2 - 1);
		const middleElem = arr[Math.floor(arr.length / 2)];
		const secondHalf = arr.filter((elem, index) => index > arr.length / 2);
		return […secondHalf, middleElem, …firstHalf]; 
	}
```
```Javascript
	const path = require('path');
	const MiniCssExtractPlugin = require('mini-css-extract-plugin');
	module.exports = {
	  entry: ['babel-polyfill', './src/JS/index.js'],
	  output: {
	    path: path.resolve(__dirname, 'dist'),
	    filename: 'bundle.js'
	  },
	  module: {
	    rules: [
	      {
	        test: /\.(sa|sc|c)ss$/,
	        use: [
	          {
	            loader: MiniCssExtractPlugin.loader
	          },
	          {
	            loader: 'css-loader'
	          },
	          {
	            loader: 'postcss-loader'
	          },
	          {
	            loader: 'sass-loader',
	            options: {
	              implementation: require('sass')
	            }
	          }
	        ]
	      },
	      {
	        test: /\.js$/,
	        exclude: /(node_modules)/,
	        use: {
	          loader: 'babel-loader',
	          options: {
	            presets: ['@babel/preset-env']
	          }
	        }
	      },
	      {
	        test: /\.(png|jpe?g|gif|svg)$/,
	        use: [
	          {
	            loader: 'file-loader',
	            options: {
	              outputPath: 'images'
	            }
	          }
	        ]
	      },
	      {
	        test: /\.(woff|woff2|ttf|otf|eot)$/,
	        use: [
	          {
	            loader: 'file-loader',
	            options: {
	              outputPath: 'fonts'
	            }
	          }
	        ]
	      }
	    ]
	  },
	  plugins: [
	    new MiniCssExtractPlugin({
	      filename: 'bundle.css'
	    })
	  ],
	  mode: 'development'
	};
```
```Javascript
  
import React from 'react';
import { Field, reduxForm } from 'redux-form';
import s from './MessageBlock.module.css';
import { FormControl } from '../../common/FormsControls/FormsControls';
import { maxLengthCreator, requiredField } from '../../../utils/validators/validators';

const maxLength100 = maxLengthCreator(100);

const MessageBlock = (props) => {
    let addMessage = (values) => {
        props.addMessage(values.message);
    }
    return (
        <ReduxMessageFrom onSubmit={addMessage} />
    )
}

const MessageForm = (props) => {
    return (
        <form action="" onSubmit={props.handleSubmit} className={s.CreateBlock}>
            <Field component={FormControl} validate={[requiredField, maxLength100]} className={s.textarea} type="text" name="message" placeholder="Yooooooooo samurai" fieldtype="textarea" />
            <button className={s.sendButton}> Send </button>
        </form>
    )
}
const ReduxMessageFrom = reduxForm({
    form: 'messageForm'
})(MessageForm);

export default MessageBlock;
```

## Experience:
 No working experience (only self coding and courses projects).

## Education:
* Online courses and Tutorials (HTML Academy, Codeacademy, The Modern JavaScript Tutorial).
* completed offline courses: “FrontEnd start” in TeachMeSkills, “ServiceNow” in EPAM;
* RSSchool: “RSSchool-2019/2020”; 

## English:
 **B1 level** (have certification of "Ispeek" language school) Keep learning.