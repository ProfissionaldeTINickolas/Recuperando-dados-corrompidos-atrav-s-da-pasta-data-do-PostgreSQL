Quando o serviço do postgres é deixado para inicializar automaticamente, o computador do cliente pegar um vírus, o cliente não for atencioso com a rotina de backup ou mandar para um técnico formatar  e ele fizer o backup simplesmente salvando a pasta do Windows para
Windows.OLD, sem fazer o backup primeiro pelo PGAdmin, 
um dos problemas que pode acontecer é corromper algum arquivo da base de dados e o cliente não ter o arquivo na extensão .backup. Este é um dos principais motivos, porém poderá ocorrer por outros.


1 – Faça uma cópia da pasta data que localiza-se no diretório de instalação onde o postgres estava antes de formatar o computador ou corromper os arquivos

2 – Verifique se existe o postgres no painel de controle > adicionar ou remover programas, se constar, desinstalar

3 – Instale novamente, utilizando a mesma versão, configurações de usuário e senha,etc.

4 –Pare o serviço do postgres, substitua a pasta data, e substitua os arquivos coincidentes, a´pós inicie o serviço novamente

Importante: Esse processo nem sempre funcionará, ele é considerado em T.I um método de tentativa de  recuperação de desastres
pois depende de vários fatores, como a integridade do arquivo movido, versão do postgres e Windows. O cliente precisa estar ciente das informações e a importância de cuidar do Backup e possuir servidores bons
