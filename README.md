<div align="center">
<img src="https://github.com/jasurhaydarovcode/card-API-react/blob/main/.github/JSON_vector_logo.svg.png?raw=true" width="129">
<img src="https://github.com/jasurhaydarovcode/card-API-react/blob/main/.github/12372044.png?raw=true" width="132">

# JSON+API
</div>


### Import API

# 1.
```jsx

function App() {

  const users = [
    {
      id: 1,
      name: "Jasur",
      age: 18,
    },
    {
      id: 2,
      name: "Ali",
      age: 22
    }
  ];
  return (
    <div>
      {users.map(user => (
        <div key={user.id}>
          <h3>{user.name}</h3>
          <p>age: {user.age}</p>
        </div>
      ))}
    </div>
  );
}

export default App;
```


# 2.

```jsx
import React from 'react'

// Your API
import cardsAPI from './API/card.json'

const App = () => {

    const Card = ({ title, desc }) => {
    return (
      <div className='m-auto'>
        <div className='border-2 border-red-800'> 
          <h2>{title}</h2>
          <p>{desc}</p>
        </div>
      </div>
    )
  }

  return (
      <>
      <div className='flex gap-5'>
        {cardsAPI.map(card => (
          <Card key={card.id} title={card.title} desc={card.desc} />
        ))}
      </div>
    </>
  )
}

export default App
```

---

### [Chat GPT](https://chatgpt.com/share/7530a3b5-2553-4b52-99be-4141aa576ebf)
