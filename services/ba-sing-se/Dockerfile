FROM arm64v8/golang:1.19.6-alpine

WORKDIR /app

COPY go.mod go.sum ./
RUN go mod download

COPY . .

RUN go build -o ba-sing-se

EXPOSE 3000

CMD ["/app/ba-sing-se"]
