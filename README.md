projeto 1
import random
lista=[0,1,2,3,4,5]
n1=random.choice(lista)
n2=(int(input('adivinhe em qual numero eu estou pensando: ')))
if n2==n1:
    print('CERTA RESPOSTA')
else:
    print('RESPOSTA ERRADA')
print(n1)

#projeto 2

n1=(int(input('vc estava dirigindo a ')))
if n1 > 80:
    print('Você foi multado  por excesso de velocidade!')
    multa=((n1-80)*7)
print('o valor da multa será de R${:.2f}'.format(multa))
print ('tenha um bom dia')





#peojeto 3

n1=(int(input('digite um número:')))
resultado= n1 % 2
if resultado==0:
    print('este número é PAR')
else:
    print('Este número é IMPAR')



#projeto 4
n1=(int(input('qual o valor do imóvel? ')))
n2=(int(input('quanto você ganha? ')))
n3=(int(input('em quantos anos pagara a fatura? ')))
n4=(n3*12)
n5=(int(n1/n4))
print(n4,'meses em parcelas')
print('vc teria que pagar',n5,'mensalmente.')
if n5>(n2*0.3):
    print('desculpe, não podemos fazer o empréstimo')
else:
    print('empréstimo liberado')



#projeto 5
n1=int(input('digite um numero'))
n2=int(input('digite outro numero'))
if n1>n2:
    print('\033[3;45;47m o primeiro numero eh maior q o segundo')
elif n2>n1:
    print('\033[1;42;45m o segundo numero eh maior q o primeiro')
else:
    print('\033[7;41;42m esses numeros sao iguais')


#projeto 6
sexo=str(input('informe seu sexo: [M/F] ').strip().upper()[0])
while sexo not in 'MmFf':
    sexo=str(input('dados inválidos, informe seu sexo: ')).strip().upper()[0]
print('{}. seu sexo foi computado no nosso banco de dados'.format(sexo))


#projeto 7
nickname=str(input('digite seu nome de usuário: '))
senha=str(input('crie sua senha: '))
while senha in nickname:
    senha=str(input('sua senha não pode ser a mesma que o nome de usuário, escolha outra senha: '))
print('nome de usuário:{}.       senha: {}, dados salvos com sucesso'.format(nickname,senha))


#projeto 8
n1= cont= conta=0
while n1!=999:
    n1=(int(input('digite um número (999 para parar): ')))
    cont+=1
    conta+=(n1)
    if n1==999:
        break
print(f"você digitou {cont-1} números e a soma deles é {conta-999}")


#projeto 9
n1=int(input('digite um número para saber sua tabuada (número negativo para parar): '))
while n1>=0:
    for c in range(1,11):
        print(f'{n1}X{c}=',n1*c)
    n1=int(input('outro valor? '))
    if n1<=-1:
       break
print("fim das operações")


