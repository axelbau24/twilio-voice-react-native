<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@twilio/voice-react-native-sdk](./voice-react-native-sdk.md) &gt; [Call](./voice-react-native-sdk.call_interface.md) &gt; [addEventListener](./voice-react-native-sdk.call_interface.addeventlistener_7_methodsignature.md)

## Call.addEventListener() method

Quality warnings changed event. Raised when a call quality warning is set or unset. All "ongoing" call quality warnings are passed to the invoked listener function.

<b>Signature:</b>

```typescript
addEventListener(qualityWarningsChangedEvent: Call.Event.QualityWarningsChanged, listener: Call.Listener.QualityWarningsChanged): this;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  qualityWarningsChangedEvent | [Call.Event.QualityWarningsChanged](./voice-react-native-sdk.call_namespace.event_enum.md) | The raised event string. |
|  listener | [Call.Listener.QualityWarningsChanged](./voice-react-native-sdk.call_namespace.listener_namespace.qualitywarningschanged_typealias.md) | A listener function that will be invoked when the event is raised. |

<b>Returns:</b>

this

- The call object.

## Example


```typescript
call.addEventListener(
  Call.Event.QualityWarningsChanged,
  (
     currentWarnings: Call.QualityWarning[],
     previousWarnings: Call.QualityWarning[]
  ) => {
    // call quality warnings have changed
  }
);
```
