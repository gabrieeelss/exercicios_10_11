01 - 
select*from tb_alunos ta 
order by ta.nome asc 
![](image.png)

02 -
select sigla, nome_curso
from tb_cursos tc 
where tc.carga_horaria = 1200
![](image-1.png)

03 -
select nome, especialidade
from tb_docentes td 
where td.especialidade = "programação"
![](image-2.png)

04 - 
select id_sala, numero_sala, capacidade
from tb_salas ts 
where ts.tipo = "teorica"
![](image-3.png)

05 - 
select sigla_turma
from tb_turmas tt 
where turno = "tarde"
![](image-4.png)

06 - 
select nome 
from tb_alunos ta 
where ta.id_aluno = 149
![](image-5.png)

07 - 
select nome_sala, numero_sala
from tb_salas ts 
where ts.capacidade = 30
![](image-6.png)

08 - 
select sigla
from tb_cursos tc 
where tc.carga_horaria = 1000
![](image-7.png)

09 - 
select nome
from tb_alunos ta 
where nome like "w%"
![](image-8.png)

10 - 
select nome, especialidade
from tb_docentes td 
where td.id_docente = 7
![](image-9.png)

11 - 
select sigla_turma
from tb_turmas tt 
where tt.turno = "noite" and tt.id_curso_fk = 2
![](image-10.png)

12 - 
select ta.nome 
from tb_alunos ta 
where ta.data_nascimento like "2005-03-12"
![](image-11.png)

13 - 
select sigla_turma
from tb_turmas tt 
where tt.id_sala_fk = 6
![](image-12.png)

14 - 
select tc.id_curso, tc.nome_curso 
from tb_cursos tc 
where tc.carga_horaria > 800
![](image-13.png)

15 - 
select td.nome 
from tb_docentes td 
where td.especialidade <> "enfermagem"
![](image-14.png)

16 - 
select ta.id_aluno, ta.nome 
from tb_alunos ta inner join tb_aluno_turma tat 
on ta.id_aluno = tat.id_aluno_fk 
where tat.id_turma_fk = 17
![](image-15.png)

17 - 
select tc.nome_curso 
from tb_cursos tc 
where tc.id_curso = 10
![](image-16.png)

18 - 
select nome
from tb_docentes td inner join tb_docente_curso tdc 
where tdc.id_curso_fk = 19
![](image-17.png)

19 - 
select tt.sigla_turma , tt.turno 
from tb_turmas tt 
where tt.id_sala_fk  = 11
![](image-18.png)

20 - 
SELECT tc.sigla, tc.nome_curso 
from tb_cursos tc inner join tb_turmas tm 
on tc.id_curso = tm.id_curso_fk 
where id_turma BETWEEN 56 and 60
 ![](image-19.png)

 21 - 
 