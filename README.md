query example :

curl "http://127.0.0.1:8983/solr/cassandra_employee/select?q=last_name:Doe&fl=last_name,first_name"

cql :

CREATE TABLE cqlintro.employee (
    company_id int,
    employee_id int,
    first_name text,
    last_name text,
    PRIMARY KEY (company_id, employee_id)
);


 company_id | employee_id | first_name | last_name
------------+-------------+------------+-----------
          1 |           1 |       John |       Doe
          1 |           2 |       Jane |       Doe
          2 |           3 |       Erik |  Davidson
          2 |           4 |        Joe |      Cool
