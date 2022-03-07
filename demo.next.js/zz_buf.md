# 后续研究:

vscode+容器


# 最近的工程:


[db].[table].[key]

# 1 table by list
db1.tb1.c1(
    cond=1/[manual], auto_cond=[dataStatus!=3], select=default
)[name_list].df

# 1 table join table
db1.tb1.c1(
    cond=1/[manual], 
    auto_cond=[dataStatus!=3], 
    select=default
)[
    db1.tb1.c2(
        cond=1/[manual], auto_cond=[dataStatus!=3], select=default
    )
].df
