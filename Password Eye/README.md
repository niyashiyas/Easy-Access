### Password Eye

- React Class Components
```Javascript
    this.state{
        showPassword:false,
    }
    <img onClick={()=>{this.setState({...this.state, showPassword: !this.state.showPassword})}} className="eye_password" src={this.state.showPassword? "https://media.geeksforgeeks.org/wp-content/uploads/20210917150049/eyeslash.png" : "https://media.geeksforgeeks.org/wp-content/uploads/20210917145551/eye.png"} alt="eye"/>
```

```Javascript
    import { useState } from 'react'
    const [showPassword, SetShowPassword] = useState('false')
    <input className="my-2 mb-4 p-1 px-2 rounded-lg" onChange={(e) => setPassword(e.target.value)} required type={showPassword? "text" : "password"} name="password" id="password" placeholder="password" />
    <img onClick={()=>SetShowPassword(!showPassword)} className="inline ml-2 w-5" src={showPassword ? "https://media.geeksforgeeks.org/wp-content/uploads/20210917150049/eyeslash.png" : "https://media.geeksforgeeks.org/wp-content/uploads/20210917145551/eye.png"} alt="eye"/>
```