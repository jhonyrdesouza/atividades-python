horas_trabalhadas = float (input('Insira aqui o valor de sua hora de trabalho:'))
horas_trabalhadas_mes = float (input('Insira aqui o valor das suas horas trabalhadas por mês:'))
numero_dependentes = int(input('Insira aqui a quantidade de dependentes:'))

salario_bruto = (horas_trabalhadas * horas_trabalhadas_mes) 
inss = (salario_bruto * 0.08)
plano_saude = (salario_bruto * 0.02) + (salario_bruto * 0.01 * numero_dependentes)
salario_liquido = (salario_bruto - inss - plano_saude)
beneficios = (850 + (salario_bruto * 0.01))

print (f'Sálario Bruto = {salario_bruto:.2f}R$\nBenefícios = {beneficios:.2f}R$')
print (f'Desconto do INSS = {inss:.2f}R$\nPlano de Saúde = {plano_saude:.2f}R$')
print (f'Sálario Líquido = {salario_liquido:.2f}R$')
