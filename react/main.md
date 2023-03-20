### Here are some of react example code. I did not spoil the fun.

`(*Note: I am open for new way of thinking to achieve perfection in coding)`

1. How many times the console.log() will be called in following code?

```
function App() {
  const [count, setCount] = useState(0);
  console.log('this line is called');
  useEffect(()=>{
    setCount((prvCount) => prvCount++)
  }, []);

  return <div className="App" />;
}
```

And how many times the same log is called if I switch line 11 to `setCount((prvCount) => ++prvCount)`?

2. Weird behavior with addEventListener and useState. Refer [here](https://codesandbox.io/s/react-16-7-alpha-forked-nqjxdm).
