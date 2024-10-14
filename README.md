# ant-design-vue-notification-bug

![issue](https://github.com/vueComponent/ant-design-vue/issues/7875)

## description

it seems like that `Holder`'s props lack some properties. 

![image](https://github.com/user-attachments/assets/4236f95d-1132-4a98-b688-b63d152ac1bf)

![image](https://github.com/user-attachments/assets/9c95dbd6-b21c-441f-baf6-60af1f5e1a8d)

the `top` property can be found in `attrs`.

![image](https://github.com/user-attachments/assets/2c4cbddd-3544-418a-a07a-ca1d0c7ea68c)

but `getStyles` would check the `props.top` instead of `attrs.top`.

![image](https://github.com/user-attachments/assets/8f78ad21-af58-4bf0-8cd1-d5b2cfd93df6)

the notification's static method doesn't have this problem.
