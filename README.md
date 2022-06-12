# Termoquimica.py
Este código foi desenvolvido para calcular funções termodinâmicas usando arquivos de saída do pacote QuantumESPRESSO - v. >6.4.1. Para configurá-lo abra um terminal e dê o comando:
                     
                     python3 setup.py
                     
Isso vai verificar se as depêndencias do  programa estão satisfeitas, caso não esteja, vai tentar instalá-las automaticamente. Em caso de falha, faça manualmente um por um,  nesta ordem.
            
                     sudo apt install python3-pip python3-pyqt5 -y
                     python3 -m pip install numpy
                     python3 -m pip install pyqt5
                     chmod u+x termoquimica.py
                     sudo ln -sf $PWD/termoquimica.py /usr/bin/termoquimica
                     
Após concluir a configuração, para executar o programa basta abrir um terminal de digitar: termoquimica

NOTAS DE USO

teclas de atalho para exibir funções separadamente: (Menu Exibir)

F7  = 'Temperatura x E_interna'\
F8  = 'Temperatura x Entropia'\
F9  = 'Temperatura x Entalpia'\
F10 = 'Temperatura x E_Gibbs'\
F11 = 'Temperatura x E_Helmholtz'

Temperatura mínima deve, obrigatóriamente, ser diferente da temperatura máxima. Caso deseje plotar os resultados para apenas um valor de T, faça da seguinte forma:

  Tmin; (Tmax = Tmin + Delta T); Delta T
  Ex: para calcular em T = 100 K, faça:
          Tmin = 100; Tmax = 110; Delta T = 10

Após inserir os dados, basta clicar em calcular que os dados serão exibidos na área de texto. 

Para salvar os dados que estão mostrados na tela clique no botão salvar, forneça um nome para o arquivo e indique o diretório para ele.
Por padrão, a área de texto é definida como somente leitura. Caso deseje editar os dados basta clicar no botão "Editar".

Caso deseje copiar os dados exibidos na área de texto, basta clicar no botão copiar.

Alternativamente ao uso da interface gráfica (gui), o usuário pode optar por uma versão em linha de comando (com funcionalidades reduzidas). Para isso basta executar o código console.py em um terminal. Este módulo necessita apenas da biblioteca matemática numpy, que pode ser instalada com o comando 
sudo apt install python3-pip
python3 -m pip install numpy
