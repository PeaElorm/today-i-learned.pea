### Understanding "dispatch" in "useReducer"
The `dispatch` function in `useReducer` is like a messanger that delivers action instructions to your state manager.

useReducer gives you two things: your current state and a dispatch function.

1. When you want to change your state, you call `dispatch` with an action.
2. The action is a message telling your reducer function what change to make.
3. The reducer follows this instructions and updates the state.

   Think of it like you are in a restaurant:
     * The initial state may be your empty table or a pack of gum on the house.
     * The waiter is the dispatch.
     * The action is your order for the food.
     * The reducer is the kitchen that prepares your order.
  
   so when you call
   ``` js
     dispatch({type:"ADD_ORDER", payload: "Pizza"})
   ```
   You are telling the reducer(kitchen) to add pizza(action) to your table(state)

   The beauty is you do not have to worry about how the state change happens - you just send messages through dispatch and the reducer takes care of updating the state correctly.

   ![image](https://github.com/user-attachments/assets/3c2de2ba-ba47-4268-bfab-23e1a077c113)
