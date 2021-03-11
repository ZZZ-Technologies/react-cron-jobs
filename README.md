# react cron jobs
React UI component to create cron expression.

## installation
```` bash
npm install --save react-cron-jobs
````
## demo
<a href="https://codesandbox.io/s/react-cron-jobs-demo-lzxwn" target="_blank"> Live demo </a>

## Usage

```javascript
import React from 'react';
import './App.css';
import CronJob from 'react-cron-jobs';

class App extends React.Component {

  myCallBackFunc(cronExp, scheduleName) {
    console.log('Cron expression for schedule ' + scheduleName + ' is ' + cronExp);
  }

  render () {
    return(
      <div>
        <CronJob onChange={this.myCallBackFunc}>
        </CronJob>
      </div>
    );
  }
}

export default App;
```

## Props

| Prop              | Type       | Description |
|-------------------|------------|-------------|
| `onChange`         | _function_  | Use this callback function to receive the cron expression for the schedule configured.  |
---

## License

MIT
