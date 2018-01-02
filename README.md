Networking Terraform Module
===========================

Reference in the main TF script as the following:

```json
{
  "module": {
    "networking": {
      "source": "github.com/snatalenko/tf_networking/?ref=v0.1.1",
      "app": "${var.app}",
      "openvpn_trusted_ips": "${var.openvpn_trusted_ips}",
      "openvpn_default_password": "${var.openvpn_default_password}",
      "openvpn_instance_key_name": "${aws_key_pair.admin.key_name}"
    }
  }
}
```

See other configuration parameters in the `variable` section of the **main.tf.json**