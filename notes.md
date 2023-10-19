No **Vscode**, eu acredito que seja possível usar o Thunder para fazer as requisições  

Dada a criação da aplicação, eu devo seguir o passo para obter o token de acesso  

Para acessar o token, no terminal, enviar essas informações. Lembrando, que é necessário substituir as variáveis
```bash
curl -X POST "https://accounts.spotify.com/api/token" \
     -H "Content-Type: application/x-www-form-urlencoded" \
     -d "grant_type=client_credentials&client_id=your-client-id&client_secret=your-client-secret"
```


A necessidade de usar um Verificador de Código  

**Authorization Code with PKCE Flow:**  
https://developer.spotify.com/documentation/web-api/tutorials/code-pkce-flow

Como estava sendo usado o JavaScript, fui em busca de algo que pudesse ser usado em Python para acelerar o processo. Encontrei um tutorial em que a moça usa Flask para o framewokr web  

**Flask**:  
https://flask.palletsprojects.com/en/3.0.x/quickstart/  
**Spotify OAuth**:  
https://www.youtube.com/watch?v=mBycigbJQzA  
**Spotipy**: https://spotipy.readthedocs.io/en/2.22.1/