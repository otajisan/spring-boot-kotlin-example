# spring-boot-kotlin-example
example of SpringBoot by Kotlin

# Health Check

```bash
⫸  curl localhost:18080/actuator/health
{"status":"UP"}
```

# Prometheus

```bash
⫸  curl -s localhost:18080/actuator/prometheus
# HELP jvm_threads_peak_threads The peak live thread count since the Java virtual machine started or peak was reset
# TYPE jvm_threads_peak_threads gauge
jvm_threads_peak_threads 43.0
# HELP jvm_threads_states_threads The current number of threads having NEW state
# TYPE jvm_threads_states_threads gauge
jvm_threads_states_threads{state="runnable",} 10.0
jvm_threads_states_threads{state="blocked",} 0.0
jvm_threads_states_threads{state="waiting",} 23.0
jvm_threads_states_threads{state="timed-waiting",} 5.0
jvm_threads_states_threads{state="new",} 0.0
...
```

# Open API
http://localhost:8080/v3/api-docs