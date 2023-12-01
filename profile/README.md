# Labrador Rover
Repositórios dos projetos utilizado para o desenvolvimento de um rover utilizando a placa Labrador. O projeto consiste na montagem de um rover utilizando a placa labrador.

## rover-api-socketio
API em tempo real que atua escutando os eventos enviados pelo usuário através do navegador. Através de uma página web que a API disponibiliza, um usuário poderá emitir comandos,
como pressionar as teclas: W, A, S e D, para controlar o rover. A API se encarrega de escutar esses eventos e de disparar outros eventos que são executados na placa Labrador que interagem diretamente
com as portas PWM para que o rover possa se movimentar (a interação com as portas PWM são realizadas no projeto **rover-remote-control**).

### Tecnologias utilizadas
- Python 3;
- FastAPI;
- WebSocket
  - Foi utilizado a lib [https://python-socketio.readthedocs.io/en/latest/index.html](python-sockeio);
- HTML, CSS e Javascript.
    
## rover-remote-control
Atua interpretando os eventos enviados pelo servidor para interagir com as portas PWM e fazer o rover se movimentar o parar.

### Tecnologias utilizadas
- Python 3;
- [https://python-socketio.readthedocs.io/en/latest/index.html](python-sockeio);
- [https://github.com/caninos-loucos/caninos-sdk](caninos-sdk)

# Referências
https://wiki.caninosloucos.org/index.php/P%C3%A1gina_principal
https://github.com/caninos-loucos/caninos-sdk
