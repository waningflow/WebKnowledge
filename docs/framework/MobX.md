# MobX

- 任何源自应用状态的东西都应该自动地获得

## 生成observable

- observable
```js
const map = observable.map({ key: "value"});

const list = observable([1, 2, 4]);

const person = observable({
    firstName: "Clive Staples",
    lastName: "Lewis"
});

const temperature = observable.box(20);
```
- @observable
```js
import { observable, computed } from "mobx";

class OrderLine {
    @observable price = 0;
    @observable amount = 1;
}
```

## 响应observable

- computed
- autorun
- when
- reaction
- observer

## 改变observable

- action
- async action & flows
- Object api

## 实用工具函数

- toJS
- extendObservable
- createAtom
- intercept & observe
- mobxUtils
    - fromPromise
    - fromResource
    - toStream
    - fromStream
    - now
    - createTransformer
    - expr

## 常用技巧
