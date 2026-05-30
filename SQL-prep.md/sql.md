
#  Question_id: 1757: Recyclable and low fats products
#  link ->   https://leetcode.com/problems/recyclable-and-low-fat-products/description/?envType=study-plan-v2&envId=top-sql-50

# 
# Question- Write a solution to find the ids of products that are both low fat and recyclable.
# Return the result table in any order.

# Solution:

''' select product_id from Products
where low_fats = "y" && recyclable = "y" '''

# %% [markdown]
# ### 584. Find customer referee
# 
# ### link -> https://leetcode.com/problems/find-customer-referee/editorial/?envType=study-plan-v2&envId=top-sql-50


# Find the names of the customer that are either:

# referred by any customer with id != 2.
# not referred by any customer.

# solution
''' SELECT name
FROM customer
WHERE referee_id!=2 OR referee_id is null; '''

#  175. Add two tables

# Link: https://leetcode.com/problems/combine-two-tables/


# Write a solution to report the first name, last name, city, and state of each person in the Person table. If the address of a personId is not present in the Address table, report null instead.
# Return the result table in any order.

''' select p.firstName, p.lastName, a.City, a.state from Person p
left join Address a 
on p.personID = a.personID'''
