# biglinux-appid

## Descrição
O `biglinux-appid` é um script Bash que auxilia na identificação do `app_id` de aplicativos rodando sob Wayland. Ele pode ser utilizado para obter informações de identificação de janelas de aplicativos e também para executar aplicativos da web no Brave com um `class` personalizado.

## Requisitos
- `bash`
- `grep`
- `brave` (para a funcionalidade `big_appid`)

## Instalação
Copie o script para um diretório no seu `$PATH`, como `/usr/local/bin/`, e dê permissão de execução:

```sh
chmod +x biglinux-appid
sudo mv biglinux-appid /usr/local/bin/
```

## Uso

### Sintaxe
```sh
biglinux-appid [OPÇÃO] [URL]
```

### Opções Disponíveis
- `--id | -i`  
  Executa `big_appid`, abrindo um aplicativo web no Brave e capturando seu `app_id`.

- `-id-web | -w`  
  Executa `big_appid_web`, filtrando a saída para encontrar o `app_id` de qualquer aplicação rodando sob Wayland.

- `--help | -h`  
  Exibe a mensagem de ajuda.

### Exemplo

- Para capturar o `app_id` de qualquer aplicativo rodando sob Wayland:
   ```sh
   biglinux-appid -w <comando_do_aplicativo>
   ```

## Licença
Este projeto está licenciado sob a licença BSD de 2 Cláusulas. Consulte o código fonte para mais detalhes.

## Autor
Desenvolvido por:  
**Marcelo (Elppans)** (<marcelo.elven@*>)  
**Vilmar Catafesta** (<vcatafesta@*>)  

