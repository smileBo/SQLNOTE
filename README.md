# SQLNOTE
sql数据库的一些笔记
--已知id的上一条数据
 
 declare @d int= (select top 1 tint from testmaxandmin where tid < 1 order by tid desc)
 select @d
--已知id的下一条数据
select top 1 tint from testmaxandmin where tid > 1 order by tid asc
