# NativeScript SerailPort Plugin

## English

Plugin for working with serail port. Based on the serialport-plugin-example wrapper, file ./release/serialport-plugin.aar over [felHR85 / UsbSerial library](https://github.com/felHR85/UsbSerial)

[Plugin creation instructions](https://www.nativescript.org/blog/plugins-and-jars)

[React Native Template](https://github.com/melihyarikkaya/react-native-serialport)

## Russian

Плагин для работы с serail port. Основан на обертке [serialport-plugin-example](https://github.com/b0939261761/serialport-plugin-example), файл `./release/serialport-plugin.aar`
над библиотекой [felHR85/UsbSerial](https://github.com/felHR85/UsbSerial)

[Инструкция содания плагина](https://www.nativescript.org/blog/plugins-and-jars)

Шаблон [React Native](https://github.com/melihyarikkaya/react-native-serialport)

```js
const onCallback = (context, intent) => {
  if (TNS_ENV !== 'production') console.info(intent.getAction());
};

serialport.on(serialport.DEVICE_ATTACHED, onCallback);
serialport.on(serialport.DEVICE_DETACHED, onCallback);
serialport.on(serialport.DEVICE_PERMISSION_GRANTED, onCallback);
serialport.on(serialport.DEVICE_PERMISSION, onCallback);
serialport.on(serialport.DEVICE_CONNECT, onCallback);
```
