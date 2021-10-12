# Termoquimica.py
Este software foi desenvolvido para calcular funções termodinâmicas. Para configurá-lo abra um terminal e dê o comando:
#   ~$ python3 setup.py
Esse comando vai verificar se as depêndencias do  programa es tão satisfeitas,ca-so não esteja, vai  instala-las automaticamente. Em caso de falha tente instalar manualmente um por um,  nesta ordem.
   ~$ sudo apt install python3-pip -y
   ~$ sudo apt install python3-pyqt5 -y
   ~$ python3 -m pip install numpy"
   ~$ python3 -m pip install pyqt5
   ~$ chmod u+x termoquimica.py
   ~$ sudo ln -sf $PWD/termoquimica.py /usr/bin/termoquimica
Após concluir a configuração, para executar o programa basta abrir um terminal de digitar: termoquimica

# NOTAS DE USO
Software programado para ler arquivos de saída das versões 6x do Quantum Espresso.
Temperatura mínima obrigatóriamente deve ser diferente da temperatura máxima. Caso deseje plotar os resultados para apenas um valor de T, faça da seguinte forma:

                    Tmin; (Tmax = Tmin + Delta T); Delta T

Após inserir os dados, basta clicar em calcular que os dados serão exibidos na área de texto.

**teclas de atalho para exibir funções separadamente: (Menu Exibir)

                    F7  = 'Temperatura x E_interna'
                    F8  = 'Temperatura x Entropia'
                    F9  = 'Temperatura x Entalpia'
                    F10 = 'Temperatura x E_Gibbs'
                    F11 = 'Temperatura x E_Helmholtz'

Para salvar os dados que estão mostrados na tela basta clicar no botão salvar, fornecer um nome para o arquivo e setar o diretório para ele.

Por padrão, a área de texto é definida como somente leitura. Caso deseje editar os dados basta clicar no botão "Editar".
