 
 
 <h1 align="center">
 <samp>
 User-Model Backend Api
 </samp>
 </h1>
 
 <p align="center">
 <samp>
 1. User - Entity
 </samp>
 <center>
 <table >
  <tr>
    <th>Property</th>
    <th>Type</th>
    <th>Remarks</th>
  </tr>
    <tr>
    <th>id</th>
    <th>number</th>
    <th>Auto-generated ( User-Id )</th>
  </tr>
    <tr>
    <th>name</th>
    <th>string</th>
    <th>Unique : true</th>
  </tr>
    <tr>
    <th>mobileno</th>
    <th>number</th>
    <th>Unique : true</th>
  </tr>
    <tr>
    <th>email</th>
    <th>string</th>
    <th>Unique : true</th>
  </tr>
    <tr>
    <th>password</th>
    <th>string</th>
  </tr>
    <tr>
    <th>Department</th>
    <th>DEPARTMENT</th>
    <th>ENUM</th>
  </tr>
    <tr>
    <th>subject</th>
    <th>string</th>
  </tr>
    <tr>
    <th>class</th>
    <th>string</th>
  </tr>
    <tr>
    <th>joindate</th>
    <th>Date</th>
    <th>Auto created at creation</th>
  </tr>
    <tr>
    <th>status</th>
    <th>STATUS</th>
    <th>ENUM</th>
  </tr>
    <tr>
    <th>activeissues</th>
    <th>number</th>
    <th>Default: 0 (Auto created at creation)</th>
  </tr>
    <tr>
    <th>totalissuessolved</th>
    <th>number</th>
    <th>Default: 0 (Auto created at creation)</th>
  </tr>
    <tr>
    <th>avgsolvedissuesperday</th>
    <th>number</th>
    <th>Default: 0 (Auto created at creation)</th>
  </tr>
    <tr>
    <th>proposedcapperday</th>
    <th>number</th>
  </tr>
 </table>
 </center>
 </p>
 
 <h2 align="center">
 <samp>
 API
 </samo>
 </h2>
<p>
<samp>
1. Create User
</samp>
<br>
<samp>
'''
POST http://localhost:4000/user
'''
</samp>
<p>
<samp>
'''
{
    "name":"rajesh",
    "mobileno": 980000020,
    "email": "rajesh@gmail.com",
    "password":"password",
    "Department":"ADACEMIC",
    "subject": "math",
    "class": "11th",
    "status": "ACTIVE",
    "proposedcapperday":45
}
'''
</samp>
</p>
</p>

<p>
<samp>
2. Update User
</samp>
  <br>
<samp>
'''
PATCH http://localhost:4000/user
'''
</samp>
<p>
<samp>
'''
{
    "email": "updated@gmail.com"
}
'''
</samp>
</p>
</p>

<p>
<samp>
3. Delete User
</samp>
  <br>
<samp>
'''
DELETE http://localhost:4000/user/{id}
'''
</samp>
</p>


<p>
<samp>
4. Get All User
</samp>
  <br>
<samp>
'''
GET http://localhost:4000/user/
'''
</samp>
</p>


<p>
<samp>
4. Get User By Id
</samp>
  <br>
<samp>
""" GET http://localhost:4000/user/{id}
  """
</samp>
</p>




