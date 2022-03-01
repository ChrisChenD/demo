## 2 apt proxy
sudo vi /etc/apt/apt.conf.d/proxy.conf
Acquire {
  HTTPS::proxy "http://127.0.0.1:8989";
}