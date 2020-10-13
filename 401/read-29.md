# React Router
We have two modes of routing `<BrowserRouter>` and `<HashRouter`
**1- BrowserRouter**
It should be used when you have a server that will handle dynamic requests (knows how to respond to any possible URI).
**2- HashRouter**
It should be used for static websites (where the server can only respond to requests for files that it knows about)

and usually, it is preferable to use a <**BrowserRouter**> but if you are sure that the website will be static it will be good to use <**HashRouter**>

1. wrappe the App

```javascript
import { BrowserRouter } from 'react-router-dom';

ReactDOM.render((
  <BrowserRouter>
    <App />
  </BrowserRouter>
), document.getElementById('root'));
```

2. Add Switch

```javascript
<Switch>
  <Route exact path='/' component={Home}/>
  {/* both /roster and /roster/:number begin with /roster */}
  <Route path='/roster' component={Roster}/>
  <Route path='/schedule' component={Schedule}/>
</Switch>
```

3. use Link

```javascript
import { Link } from 'react-router-dom'
function Header() {
  return (
    <header>
      <nav>
        <ul>
          <li><Link to='/'>Home</Link></li>
          <li><Link to='/roster'>Roster</Link></li>
          <li><Link to='/schedule'>Schedule</Link></li>
        </ul>
      </nav>
    </header>
  );
}
```
