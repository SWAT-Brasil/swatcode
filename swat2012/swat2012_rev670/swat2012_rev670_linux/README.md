#Executáveis SWAT2012 rev670 em Linux
##Versões:
* __swat2012_rev670_linux_static__: em caso de dúvida utilize essa versão. Executavel para linux com glibfortran interno, compilado de forma estática. Utilize esse executavel caso vc tenha algum tipo de erro de glibfortran não encontrado ou se quiser garantir que funcione em qualquer maquina linux.
* __swat2012_rev670_linux__: executavel compilado com carregamento dinâmico da biblioteca glibfortran, que deve estar instalada no computador. Como não tem a biblioteca internamente, ste arquivo é um pouco menor que o executavel com bibliotécia estática.
###Problemas conhecidos:
* problema de falta de permissão de execução. No Linux o arquivo precisa ter permissão de execução para funcionar.
* verificar se o arquivo de projeto _tmp1.tmp_ está correto. Em alguns projetos o arquivo esta nomeado como _Tmp1.Tmp_, oque funciona em Windows, mas não em Linux. Renomear o arquivo para _tmp1.tmp_ para corrigir o problema. Essa alteração não deve impedir o projeto de funcionar em Windows.
* O formato dos arquivos em Windows e Linux podem ser diferentes dependendo da vesão que voce utiliza. Caso tenha algum erro de fim de linha ou de arquivo pode ser necessário alterar o formato dos arquivos. Utilize o comando __dos2unix *__  para converter os arquivos de projetos originais do Windos para Linux.
