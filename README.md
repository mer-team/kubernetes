# kubernetes
k8s files used on project deployment

## Files
`0-namespace.yaml` - Set up the `namespace` <br>
`1-persistentvolume.yaml` - Set up the `Persistent Volume` with `1Gi` in `\Audios` <br>
`2-persistentvolumeclaim.yaml` - Claim the space for the `Persistent Volume` <br>
`api-deployment.yaml` - Deploy the `api` Image <br>
`api-service.yaml` - Set up the `api` Service to run on `30080` port <br>
`database-configmap.yaml` - Configmap with the `database` config <br>
`database-deployment.yaml` - Deploy the `database` Image <br>
`database-service.yaml` - Set up the `database` Service to run on `` port <br>
`featextraction-deployment.yaml` - <br>
`frontend-deployment.yaml` - <br>
`frontend-service.yaml` - Set up the `frontend` Service <br>
`musicclass-deployment.yaml` - Deploy the `Music Classifier` Image <br>
`rabbit-deployment.yaml` - Deploy the `RabbitMQ` Image <br>
`rabbit-service.yaml` - Set up the `rabbitMQ` Service <br>
`vidextrator-deployment.yaml` - Deploy the `Video Extractor` Image

## Services
| Service | Port | nodePort |
| --- | :---: | :---: |
| API | 8000 | 30080 |
| Database | 3306 | --- |
| Frontend | 3000 | 30090 |
| RabbitMQ | 15672 <br> 5672 | --- |