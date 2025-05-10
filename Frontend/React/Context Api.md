# Context Api
If you already know about props in React, you will realise after a few usage or applications that it becomes difficult when the child component is not directly under the component that has the data(props). 
There are also cases that more than one components need that same data. Thats when Context API comes in; multiple components having access to the same props at a higher level making the props globally available.
![Image](https://github.com/user-attachments/assets/b5546b9a-6864-4368-a482-ab62ac4ddc14)

### How to create and use a context in React 
1. you need the Provider and the consumer
2. Wrap the provider around App.jsx so all the children components can have access.
3. Use context sparingly. Only use it when the data is actually global. Overusing it can cuase performance issues and cause complications 
