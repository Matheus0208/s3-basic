# S3 Básico

Exemplos simples de como enviar, baixar e apagar arquivos no **Amazon S3** usando a **AWS CLI**.

> Baseado no tutorial [tutorial-s3-basico](https://github.com/UmInventorQualquer/tutorial-s3-basico), do canal *Um Inventor Qualquer*.

## Estrutura

```
.
├── .gitignore
└── scripts/
    ├── files/          # imagens de exemplo usadas nos testes
    ├── config.json     # região e profile
    └── package.json    # dependências do AWS SDK
```

## Comandos

**Upload**
```bash
aws s3 cp ./files/philippine-coins-1483943.jpg s3://seu-bucket/ --profile tutorials3
```

**Download**
```bash
aws s3 cp s3://seu-bucket/philippine-coins-1483943.jpg ./downloads/ --profile tutorials3
```

**Delete**
```bash
aws s3 rm s3://seu-bucket/philippine-coins-1483943.jpg --profile tutorials3
```
