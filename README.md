# surveysite
<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<link rel="stylesheet" type="text/css" href="styles.css">
		<title>Student Feedback - Campus</title>
	</head>

	<body>
		<header>
			<h1>DEPARTMENT OF COMPUTER SCIENCE</h1>
			
			<nav>
				<ul>
					<li><a href="csDeptInfo.html" >Home</a></li>
					<li><a href="" class="current" >Student Survey Page</a></li>
					<li><a href="index.html" >Welcome Page</a></li>
				</ul>
			</nav>
		</header>
		
		<div id="body_wrapper" style="text-align: left; height: 700px" >
			<h2 style="color: silver; font-size: 20px;">Student Survey Form</h2>
			
			<p style="font-size: 15px;">Please fill this form to provide feedback about the campus visit:</p>
			
			<form id="studentSurveyForm" method="post" action="" autocomplete="on" 
				style="font-family:arial,helvetica,sans-serif; font-size:12px; line-height:16px; font-style:normal;">
				<table id="studentSurveyTable" summary="This table is to take information from the students about their campus visit" >
					<tbody>
						<tr>
							<td style="border-top: 5px solid rgb(150, 139, 139); padding-top: 15px;">
								<label>Last Name</label>
							</td>
							<td style="border-top: 5px solid rgb(150, 139, 139); padding-top: 15px;">
								<label>First Name</label>
							</td>
							<td style="border-top: 5px solid rgb(150, 139, 139); padding-top: 15px;">
								<label>Middle Name</label>
							</td>
						</tr>
						<tr>
							<td>
								<input type="text" id="lastName" name="lastName" maxlength="50" required="required" 
									placeholder="mareddy" autofocus="autofocus" />
							</td>
							<td>
								<input type="text" id="firstName" name="firstName" maxlength="50" required="required" placeholder="Tejashwini" />
							</td>
							<td>
								<input type="text" id="middleName" name="middleName" maxlength="50" required="required" placeholder="balaji" />
							</td>
						</tr>
						
						<tr>
							<td>
								<label>Street Address</label>
							</td>
						</tr>
						<tr>
							<td colspan="2">
								<input type="text" id="streetAddr" name="streetAddr" maxlength="100" size="47" />
							</td>
						</tr>
						
						<tr>
							<td>
								<label>City</label>
							</td>
							<td>
								<label>State</label>
							</td>
							<td>
								<label>ZipCode</label>
							</td>
						</tr>
						<tr>
							<td>
								<input type="text" id="city" name="city" maxlength="35" />
							</td>
							<td>
								<input type="text" id="state" name="state" maxlength="35" />
							</td>
							<td>
								<input type="text" id="zipCode" name="zipCode" maxlength="5" placeholder="#####" />
							</td>
						</tr>
						
						<tr>
							<td>
								<label>Telephone Number</label>
							</td>
							<td>
								<label>Email Address</label>
							</td>
						</tr>
						<tr>
							<td>
								<input type="tel" id="telNum" name="telNum" placeholder="(###) ###-####" pattern="\(\d{3}\) +\d{3}-\d{4}" />
							</td>
							<td>
								<input type="email" id="emailAddr" name="emailAddr" maxlength="100" placeholder="username@domain.com" required="required" />
							</td>
						</tr>
						
						<tr>
							<td>
								<label>Graduation Month</label>
							</td>
							<td>
								<label>Graduation Year</label>
							</td>
						</tr>
						<tr>
							<td>
								<input type="text" id="gradMonth" name="gradMonth" placeholder="Select a month" list="months" />
								<datalist id="months">
									<option value="January">
									<option value="February">
									<option value="March">
									<option value="April">
									<option value="May">
									<option value="June">
									<option value="July">
									<option value="August">
									<option value="September">
									<option value="October">
									<option value="November">
									<option value="December">
								</datalist>
							</td>
							<td>
								<input type="text" id="gradYear" name="gradYear" />
							</td>
						</tr>
						
						<tr>
							<td colspan="2">
								<label>URL</label>
							</td>
							<td>
								<label>Date of Survey</label>
							</td>
						</tr>
						<tr>
							<td colspan="2">
								<input type="url" id="url" name="url" size="47" placeholder="http:github.com" />
							</td>
							<td>
								<input type="date" id="dateOfSurvey" name="dateOfSurvey" />
							</td>
						</tr>
						
						<tr >
							<td colspan="5" style="border-top: 5px solid rgb(150, 139, 139); padding-top: 15px;">
								<label>Please check the things that you like about the campus</label>
							</td>
						</tr>
						<tr>
							<td colspan="5">
								<input type="checkbox" id="students" name="likings" >Students
								<input type="checkbox" id="location" name="likings" >Location
								<input type="checkbox" id="campus" name="likings" >Campus
								<input type="checkbox" id="atmoshpere" name="likings" >Atmosphere
								<input type="checkbox" id="dormRooms" name="likings">Dorm Rooms
								<input type="checkbox" id="sports" name="likings" >Sports
							</td>
						</tr>
						
						<tr>
							<td colspan="5">
								<label>How did you become interested in Mahatma gandhi university?</label>
							</td>
						</tr>
						<tr>
							<td colspan="5">
								<input type="radio" id="friends" name="interest" >Friends
								<input type="radio" id="television" name="interest" >Television
								<input type="radio" id="internet" name="interest" >Internet
								<input type="radio" id="other" name="interest" >Other
							</td>
						</tr>
						
						<tr>
							<td colspan="5">
								<label>Additional Comments</label>
							</td>
						</tr>
						<tr>
							<td colspan="5">
								<textarea rows="5" cols="50" placeholder="Enter your comments here (if any)"></textarea>
							</td>
						</tr>
						
						<tr>
							<td colspan="5" style="border-top: 5px solid rgb(150, 139, 139); padding-top: 15px; text-align: center;">
								<input type="reset" id="resetBtn" name="resetBtn" value="RESET" >
								<input type="submit" id="submitBtn" name="submitBtn" value="SUBMIT">
							</td>
						</tr>
					</tbody>
				</table>
			</form>
			
			<div id="bottom1" style="top: 555px; right: 90px; position: fixed;">
				<a href="http://www.gmu.edu/" target="_blank" >
					<img src="images/GMU.jpg" alt="GMU logo" style="height: 100px; width: 100px; float: right;">
				</a>
			</div>
		</div>
		
		<div id="footer" style="text-align: center;" >
			<strong>&copy; 2014 Derick Augustine Coutinho</strong>
		</div>
	</body>
</html>
