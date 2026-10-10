# Mission Reflection

## 1. Why is it important to check the host server's resources even if your containers are running perfectly?
All containers use the RAM, CPU, and disk of the host server. Even if my container looks fine, the server can still run out of resources. If that happens, every container can slow down or crash. In this lab, I used free -h and df -h to check that the server had enough memory and storage before the traffic came.

## 2. If a user complains that they cannot log into a web application, how would the docker logs command help you solve the problem?
I would run docker logs to see what happened when the user tried to log in. The logs show error messages and codes, like 401 or 500, and the time they happened. This helps me find the real cause instead of guessing, so I can fix the problem faster.

## 3. What is the difference between monitoring logs (Checkpoint 4) and monitoring metrics (Checkpoint 5)?
Logs tell me what happened. For example, my logs showed three successful 200 requests and one 404 error. Metrics tell me how much the container is using. My docker stats showed 2.73MiB of memory and 0.00% CPU. Logs are like a diary of events, while metrics are like a meter that shows numbers.

## 4. How do you think large enterprise companies monitor thousands of containers at the same time?
Big companies cannot check thousands of containers by hand. They use Prometheus to collect metrics from all the containers automatically. Then they use Grafana to show the data on dashboards and send alerts when something goes wrong. This way, the team can see problems quickly in one place.

## 5. How has your ability to troubleshoot Linux environments improved?
Before this lab, I only knew basic commands. Now I can check memory with free -h, disk space with df -h, and CPU with top. I also learned how to read logs and find the 404 line myself. I feel more confident because I can use real data to check if a server is healthy.

*AI disclosure: I used AI to help me understand the steps and improve my writing hehehehe, no to pax silica but also big no to english karabaw*
