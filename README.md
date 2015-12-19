# FastGrep
web based realtime log streamer

# setup

edit config.js for your log file pattern

```js
exports.config = {
  publish_url: 'http://localhost:3000/',
  watch_dir: [
    '/var/log/',
    '/path/to/my/log/directory',
  ],
  file_pattern: [
    /(?:<name>\w+)\.(?:<year>\d{4})(?:<month>\d{2})(?:<day>\d{2})\.log/,
  ],
};
```

custom your config.js:
FASTGREP_CONFIG_PATH defaults: './'

```bash
node FASTGREP_CONFIG_PATH=/path/to/my/conf/dir
```

inspired by [pupergpre](https://github.com/bobrik/pupergrep)
