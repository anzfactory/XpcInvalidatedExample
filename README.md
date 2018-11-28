# XpcInvalidatedExample

"The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated."

というエラーが発生するサンプル

## 環境

Xcode v10.1  
Cocoapods v1.5.3

## 再現方法

Cocoapods で下記のものをいれる

- Firebase/Core
- Firebase/AdMob

あとは iOS 12 のシミュレータで起動するだけ

### エラー内容

```
2018-11-28 20:16:24.699168+0900 XpcInvalidatedExample[23134:165023] [Client] Remote object proxy returned error: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.699339+0900 XpcInvalidatedExample[23134:165023] [Client] Remote object proxy returned error: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.699352+0900 XpcInvalidatedExample[23134:165028] [Client] Sending selectors failed with: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.699462+0900 XpcInvalidatedExample[23134:165024] [Client] Synchronous remote object proxy returned error: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.699467+0900 XpcInvalidatedExample[23134:165028] [Client] Sending selectors failed with: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.699614+0900 XpcInvalidatedExample[23134:165024] [NetworkInfo] Descriptors query returned error: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.700198+0900 XpcInvalidatedExample[23134:165028] [Client] Remote object proxy returned error: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.700389+0900 XpcInvalidatedExample[23134:165023] [Client] Sending selectors failed with: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.700389+0900 XpcInvalidatedExample[23134:165024] [Client] Synchronous remote object proxy returned error: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.700831+0900 XpcInvalidatedExample[23134:165024] [NetworkInfo] Descriptors query returned error: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.701465+0900 XpcInvalidatedExample[23134:165024] [Client] Synchronous remote object proxy returned error: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.701530+0900 XpcInvalidatedExample[23134:165023] [Client] Remote object proxy returned error: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.701799+0900 XpcInvalidatedExample[23134:165024] [NetworkInfo] Descriptors query returned error: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
2018-11-28 20:16:24.702008+0900 XpcInvalidatedExample[23134:165028] [Client] Sending selectors failed with: Error Domain=NSCocoaErrorDomain Code=4099 "The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated." UserInfo={NSDebugDescription=The connection to service named com.apple.commcenter.coretelephony.xpc was invalidated.}
```

### 補足

- 実機だとエラーはでない（ので、気にしないで良い？🤔
- プロジェクト自体は SingleApp でつくって何も手入れをしていない
