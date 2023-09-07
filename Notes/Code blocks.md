---
up: "[[Home]]"
---


Internally uses prismjs. All supported languages can be found [here](https://prismjs.com/#supported-languages)

```go
package main

import "fmt"

func main() {
	fmt.Println("Hello, 世界")
}
```

```jsx
<div>
	{content.items.map((item) => {
		<Item name={item.name} />
	})}
</div>
```

```yaml
spec:
  type: NodePort
  selector:
    app: posts
  ports:
    - name: post
      protocol: TCP
      port: 4000
      targetPort: 4000

```

```rust
fn main() {
    println!("Hello World!");
}
```

```dockerfile
FROM [python:3.8-slim](https://hub.docker.com/_/python)

COPY . /app

WORKDIR /app

RUN apt-get update && 
apt-get install -y \
build-essential \
python3-dev \
python3-setuptools \
gcc \
make

# Create a virtual environment in /opt
RUN python3 -m venv /opt/venv

# Install requirments to new virtual environment
RUN /opt/venv/bin/pip install -r requirements.txt

# purge unused
RUN apt-get remove -y --purge make gcc build-essential \
&& apt-get autoremove -y \
&& rm -rf /var/lib/apt/lists/*

# make entrypoint.sh executable
RUN chmod +x entrypoint.sh

CMD [ "./entrypoint.sh" ]
```