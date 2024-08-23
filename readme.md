# Flask Hello World Application

## Kurulum ve Çalıştırma

### Docker İle Çalıştırma

1. Docker imajını oluşturun:
    ```bash
    docker build -t my-flask-app .
    ```
2. Docker imajını çalıştırın:
    ```bash
    docker run -p 50100:50100 my-flask-app
    ```
3. Web tarayıcınızda `http://localhost:50100` adresine giderek uygulamayı görüntüleyin.

### Kubernetes Üzerinde Çalıştırma

1. Deployment ve Service dosyalarını uygulayın:
    ```bash
    kubectl apply -f deployment.yaml
    kubectl apply -f service.yaml
    ```
2. Uygulamanızın IP adresini veya DNS ismini alın:
    ```bash
    kubectl get services
    ```

### Pods

Pod sayısını artırmak için replicas değerini deployment.yaml dosyasında değiştirebilirsiniz.

## Docker Hub

Docker Hub’daki imaj: `dtmypr/my-flask-app`
