# poor man's pinger

```bash
for i in {1..500}; do wget http://localhost:5100/sleep100 >/dev/null; sleep 10; done
```

and now go to your wonderful monitoring tool, check metrics, be happy

[bash], [ping]
