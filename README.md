# element-theme-customer
Customer element ui color theme width css variables

## Start
```javascript
npm install
```
This repository's target is to customer element-ui's color theme with css variables. So that you can toggle color theme by changing css variables without import more stylesheets.
In this project I replace all the `mix` function in sass with the css variables.The first 16 colors is important.The others is blended by two of the important colors and the midpoints is 9.  
You can run `npm run build-t` to build css files and include in your project. In this css files there will be 'light' and 'dark' class.You can customer it in the `variables.scss` file.
In the fulture I'll point out the color variables in the place where it is used.A components preview will comming soon.

## Color Variables
```scss
$colors:(
  primary-color: #409EFF,
  background-color-primary: #ffffff,
  background-color: #ffffff,
  background-color-secondary: #ffffff,
  border-color-primary: #DCDFE6,     
  border-color-base: #E4E7ED,          
  border-color: #EBEEF5, 
  border-color-secondary: #F2F6FC,
  success-color: #67C23A,
  warning-color: #E6A23C,
  danger-color: #F56C6C,
  info-color: #909399,
  text-color-primary:#303133,        
  text-color:#606266,       
  text-color-secondary: #909399,     
  text-color-placeholder: #C0C4CC,

  color-black: #000000,

  /*secondary http://https://meyerweb.com midpoints:9 */
  /* https://www.colorhexa.com/color-blend for color mix*/
  color-primary-light-1: #53a8ff, /*mix($--color-white, $--color-primary, 10%)*/
  color-primary-light-2: #66b1ff, /*mix($--color-white, $--color-primary, 20%)*/
  color-primary-light-3: #79bbff, /*mix($--color-white, $--color-primary, 30%)*/
  color-primary-light-4: #8cc5ff, /*mix($--color-white, $--color-primary, 40%)*/
  color-primary-light-5: #a0cfff, /*mix($--color-white, $--color-primary, 50%)*/
  color-primary-light-6: #b3d8ff, /*mix($--color-white, $--color-primary, 60%)*/
  color-primary-light-7: #c6e2ff, /*mix($--color-white, $--color-primary, 70%)*/
  color-primary-light-8: #d9ecff, /*mix($--color-white, $--color-primary, 80%)*/
  color-primary-light-9: #ecf5ff, /*mix($--color-white, $--color-primary, 90%)*/

  color-primary-dark-1: #3A8EE6, /*mix($--color-black, $--color-primary, 10%)*/
  color-primary-dark-2: #337ECC, /*mix($--color-black, $--color-primary, 20%)*/
  color-primary-dark-3: #2D6FB3, /*mix($--color-black, $--color-primary, 30%)*/
  color-primary-dark-4: #265F99, /*mix($--color-black, $--color-primary, 40%)*/
  color-primary-dark-5: #204F80, /*mix($--color-black, $--color-primary, 50%)*/
  color-primary-dark-6: #1A3F66, /*mix($--color-black, $--color-primary, 60%)*/
  color-primary-dark-7: #132F4D, /*mix($--color-black, $--color-primary, 70%)*/
  color-primary-dark-8: #0D2033, /*mix($--color-black, $--color-primary, 80%)*/
  color-primary-dark-9: #06101A, /*mix($--color-black, $--color-primary, 90%)*/

  color-success-light-1: #76C84E ,/*mix($--color-white, $--color-success, 10%)*/
  color-success-light-2: #85CE61 ,/*mix($--color-white, $--color-success, 20%)*/
  color-success-light-3: #95D475 ,/*mix($--color-white, $--color-success, 30%)*/
  color-success-light-4: #A4DA89 ,/*mix($--color-white, $--color-success, 40%)*/
  color-success-light-5: #B3E19D ,/*mix($--color-white, $--color-success, 50%)*/
  color-success-light-6: #C2E7B0 ,/*mix($--color-white, $--color-success, 60%)*/
  color-success-light-7: #D1EDC4 ,/*mix($--color-white, $--color-success, 70%)*/
  color-success-light-8: #E1F3D8 ,/*mix($--color-white, $--color-success, 80%)*/
  color-success-light-9: #F0F9EB ,/*mix($--color-white, $--color-success, 90%)*/

  color-success-dark-1: #5DAF34 ,/*mix($--color-black, $--color-success, 10%)*/
  color-success-dark-2: #529B2E ,/*mix($--color-black, $--color-success, 20%)*/
  color-success-dark-3: #488829 ,/*mix($--color-black, $--color-success, 30%)*/
  color-success-dark-4: #3E7423 ,/*mix($--color-black, $--color-success, 40%)*/
  color-success-dark-5: #34611D ,/*mix($--color-black, $--color-success, 50%)*/
  color-success-dark-6: #294E17 ,/*mix($--color-black, $--color-success, 60%)*/
  color-success-dark-7: #1F3A11 ,/*mix($--color-black, $--color-success, 70%)*/
  color-success-dark-8: #15270C ,/*mix($--color-black, $--color-success, 80%)*/
  color-success-dark-9: #0A1306 ,/*mix($--color-black, $--color-success, 90%)*/

  color-warning-light-1: #E9AB50,/*mix($--color-white, $--color-warning, 10%)*/
  color-warning-light-2: #EBB563,/*mix($--color-white, $--color-warning, 20%)*/
  color-warning-light-3: #EEBE77,/*mix($--color-white, $--color-warning, 30%)*/
  color-warning-light-4: #F0C78A,/*mix($--color-white, $--color-warning, 40%)*/
  color-warning-light-5: #F3D19E,/*mix($--color-white, $--color-warning, 50%)*/
  color-warning-light-6: #F5DAB1,/*mix($--color-white, $--color-warning, 60%)*/
  color-warning-light-7: #F8E3C5,/*mix($--color-white, $--color-warning, 70%)*/
  color-warning-light-8: #FAECD8,/*mix($--color-white, $--color-warning, 80%)*/
  color-warning-light-9: #FDF6EC,/*mix($--color-white, $--color-warning, 90%)*/

  color-warning-dark-1: #CF9236,/*mix($--color-black, $--color-warning, 10%)*/
  color-warning-dark-2: #B88230,/*mix($--color-black, $--color-warning, 20%)*/
  color-warning-dark-3: #A1712A,/*mix($--color-black, $--color-warning, 30%)*/
  color-warning-dark-4: #8A6124,/*mix($--color-black, $--color-warning, 40%)*/
  color-warning-dark-5: #73511E,/*mix($--color-black, $--color-warning, 50%)*/
  color-warning-dark-6: #5C4118,/*mix($--color-black, $--color-warning, 60%)*/
  color-warning-dark-7: #453112,/*mix($--color-black, $--color-warning, 70%)*/
  color-warning-dark-8: #2E200C,/*mix($--color-black, $--color-warning, 80%)*/
  color-warning-dark-9: #171006,/*mix($--color-black, $--color-warning, 90%)*/

  color-danger-light-1: #F67B7B,/*mix($--color-white, $--color-danger, 10%)*/
  color-danger-light-2: #F78989,/*mix($--color-white, $--color-danger, 20%)*/
  color-danger-light-3: #F89898,/*mix($--color-white, $--color-danger, 30%)*/
  color-danger-light-4: #F9A7A7,/*mix($--color-white, $--color-danger, 40%)*/
  color-danger-light-5: #FAB6B6,/*mix($--color-white, $--color-danger, 50%)*/
  color-danger-light-6: #FBC4C4,/*mix($--color-white, $--color-danger, 60%)*/
  color-danger-light-7: #FCD3D3,/*mix($--color-white, $--color-danger, 70%)*/
  color-danger-light-8: #FDE2E2,/*mix($--color-white, $--color-danger, 80%)*/
  color-danger-light-9: #FEF0F0,/*mix($--color-white, $--color-danger, 90%)*/

  color-danger-dark-1: #DD6161,/*mix($--color-black, $--color-danger, 10%)*/
  color-danger-dark-2: #C45656,/*mix($--color-black, $--color-danger, 20%)*/
  color-danger-dark-3: #AC4C4C,/*mix($--color-black, $--color-danger, 30%)*/
  color-danger-dark-4: #934141,/*mix($--color-black, $--color-danger, 40%)*/
  color-danger-dark-5: #7B3636,/*mix($--color-black, $--color-danger, 50%)*/
  color-danger-dark-6: #622B2B,/*mix($--color-black, $--color-danger, 60%)*/
  color-danger-dark-7: #4A2020,/*mix($--color-black, $--color-danger, 70%)*/
  color-danger-dark-8: #311616,/*mix($--color-black, $--color-danger, 80%)*/
  color-danger-dark-9: #190B0B,/*mix($--color-black, $--color-danger, 90%)*/

  color-info-light-1: #9B9EA3,/*mix($--color-white, $--color-info, 10%)*/
  color-info-light-2: #A6A9AD,/*mix($--color-white, $--color-info, 20%)*/
  color-info-light-3: #B1B3B8,/*mix($--color-white, $--color-info, 30%)*/
  color-info-light-4: #BCBEC2,/*mix($--color-white, $--color-info, 40%)*/
  color-info-light-5: #C8C9CC,/*mix($--color-white, $--color-info, 50%)*/
  color-info-light-6: #D3D4D6,/*mix($--color-white, $--color-info, 60%)*/
  color-info-light-7: #DEDFE0,/*mix($--color-white, $--color-info, 70%)*/
  color-info-light-8: #E9E9EB,/*mix($--color-white, $--color-info, 80%)*/
  color-info-light-9: #F4F4F5,/*mix($--color-white, $--color-info, 90%)*/

  color-info-dark-1: #82848A,/*mix($--color-black, $--color-info, 10%)*/
  color-info-dark-2: #73767A,/*mix($--color-black, $--color-info, 20%)*/
  color-info-dark-3: #65676B,/*mix($--color-black, $--color-info, 30%)*/
  color-info-dark-4: #56585C,/*mix($--color-black, $--color-info, 40%)*/
  color-info-dark-5: #484A4D,/*mix($--color-black, $--color-info, 50%)*/
  color-info-dark-6: #3A3B3D,/*mix($--color-black, $--color-info, 60%)*/
  color-info-dark-7: #2B2C2E,/*mix($--color-black, $--color-info, 70%)*/
  color-info-dark-8: #1D1D1F,/*mix($--color-black, $--color-info, 80%)*/
  color-info-dark-9: #0E0F0F,/*mix($--color-black, $--color-info, 90%)*/

  slider-button-hover-color: #3e99f7, /* mix($--color-primary, black, 97%) */
  el-tree-node-content-highlight: #f0f7ff, /* mix($--color-white, $--color-primary, 92%) */
  dropdown-button-before: #6e6f73, /* mix($--button-default-border-color, transparent, 50%); */
  table-striped-background: #FAFAFA
);
```
