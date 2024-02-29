# Grafana Dashboard

## Follow below steps.

1. Run the prometheus and flask server using [flask_prometheus](https://github.com/akhil9294/flask_prometheus) repo.
2. Run docker container using below command.
    - docker run -d -p 3000:3000 --name=grafana grafana/grafana-oss
3. Import datasource to grafana dashboard
    - Credentials: admin/admin
    - Goto Grafana Home page
    - Click "Add your first data source"
    - Select "Prometheus" data source
    - Provide the name to datasource
    - Add Prometheus server URL (https://prometheus-server-ip:9090)
    - Click "Save and Test" at the bottom of the page
4. Import grafana dashboard using config file
    - Click on "Create your first dashboard"
    - Click on "Import dashboard"
    - Select the config file present in this repo
    - Select the folder from the dropdown
    - Select the datasource created in step 3 above
    - Click on Load button

5. Play around