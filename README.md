# Assignment-FinalProj
SQL code create database
show databases;
use jeffdatabase;
CREATE TABLE if not exists builds_id 
( id int(15), 
wizard_name varchar(46), 
build_name varchar(46), 
age_of_build int(5), 
network_number_bit_size int(4), 
network_location char(74) 
);
CREATE TABLE if not exists employees 
( id int(5), 
name_f varchar(46), 
dept varchar(46), 
age int(2), 
salary int(10), 
location varchar(46) 
);
CREATE TABLE if not exists category 
( id int(15), 
wizard_name varchar(46), 
build_name varchar(46), 
age_of_build int(5), 
network_number int(6), 
network_location char(74) 
);

INSERT INTO category
(id, wizard_name, build_name, age_of_build, network_number, network_location)
VALUES (01, 'OneNation_Repo', 'Lobo', '2017', '156', 'http://www.onenation.info/Repo/'),
(02,'TurboTv_Repo', 'Turbo', '2017', 260, 'http://turbojtv.com/repo/'),
(03,'SG_Repo', 'Stealth', '2018', 264, 'http://sgwizard.96.lt/'),
(04, 'AJ_Repo', 'Xontech_Light', '2018', 371, 'http://ajbuilds.uk/repo/'), 
(05,'TeslaBuilds_Repo', 'Aeon_Tesla', '2018', 150, 'http://theteslabuilds.com'),
(06,'SupremeBuilds_Repo', 'Titanium', '2018', 120, 'http://repo.supremebuilds.com'),
(07,'DurexWizard_Repo', 'Durex', '2018', 470, 'http://www.drxbld.com/wiz/'),
(08,'NoLimitsWizard_Repo', 'No Limits Magic', '2018', 285, 'http://www.nolimitswiz.appboxes.co/'),
(09,'KodiGeeksWizard_Repo', 'Xenon', '2018', 405, 'http://repo.kodigeeks.com/'),
(10,'FireTvGuruWizard_Repo', 'Fire Tv Guru', '2018', 335, 'http://firetvguru.net/fire'),
(11,'Genie TV Repo Wizard', 'Equinox', '2018', 410, 'http://genietv.co.uk/repo/'),
(12,'Misfit Mods Repo', 'Atomic Reborn', '2018', 410, 'http://misfitmods.com/mmwiz/'),
(13,'Warlock Wizard', 'Warlock', '2018', 100, 'http://warlockmedia.eu/warlockwizard/'),
(14,'Wookie Repo and Wizard', 'Wookie', '2018', 200, 'http://wizwookiespm.com'),
(15,'Fire TV Guru', 'Pulse CCM', '2018', 182, 'http://firetvguru.net/fire');


CREATE TABLE if not exists data_location 
( data_id int(5), 
name_f varchar(46), 
dept varchar(46), 
age int(2), 
bit_size int(10), 
location varchar(46) 
);

INSERT INTO data_location
(data_id, name_f, dept, age, bit_size, location)
VALUES (01, 'OneNation_Repo', 'Lobo', '2017', '156', 'http://www.onenation.info/Repo/'),
(02,'TurboTv_Repo', 'Turbo', '2017', 260, 'http://turbojtv.com/repo/'),
(03,'SG_Repo', 'Stealth', '2018', 264, 'http://sgwizard.96.lt/'),
(04, 'AJ_Repo', 'Xontech_Light', '2018', 371, 'http://ajbuilds.uk/repo/'), 
(05,'TeslaBuilds_Repo', 'Aeon_Tesla', '2018', 150, 'http://theteslabuilds.com'),
(06,'SupremeBuilds_Repo', 'Titanium', '2018', 120, 'http://repo.supremebuilds.com'),
(07,'DurexWizard_Repo', 'Durex', '2018', 470, 'http://www.drxbld.com/wiz/'),
(08,'NoLimitsWizard_Repo', 'No Limits Magic', '2018', 285, 'http://www.nolimitswiz.appboxes.co/'),
(09,'KodiGeeksWizard_Repo', 'Xenon', '2018', 405, 'http://repo.kodigeeks.com/'),
(10,'FireTvGuruWizard_Repo', 'Fire Tv Guru', '2018', 335, 'http://firetvguru.net/fire'),
(11,'Genie TV Repo Wizard', 'Equinox', '2018', 410, 'http://genietv.co.uk/repo/'),
(12,'Misfit Mods Repo', 'Atomic Reborn', '2018', 410, 'http://misfitmods.com/mmwiz/'),
(13,'Warlock Wizard', 'Warlock', '2018', 100, 'http://warlockmedia.eu/warlockwizard/'),
(14,'Wookie Repo and Wizard', 'Wookie', '2018', 200, 'http://wizwookiespm.com'),
(15,'Fire TV Guru', 'Pulse CCM', '2018', 182, 'http://firetvguru.net/fire');


CREATE TABLE if not exists wizard_info 
( wiz_id int(15), 
wizard_name varchar(46), 
build_name varchar(46), 
age_of_build int(5), 
network_number int(46), 
network_location char(76) 
);

INSERT INTO wizard_info
(wiz_id, wizard_name, build_name, age_of_build, network_number, network_location)
VALUES (01, 'OneNation_Repo', 'Lobo', '2017', '156', 'http://www.onenation.info/Repo/'),
(02,'TurboTv_Repo', 'Turbo', '2017', 260, 'http://turbojtv.com/repo/'),
(03,'SG_Repo', 'Stealth', '2018', 264, 'http://sgwizard.96.lt/'),
(04, 'AJ_Repo', 'Xontech_Light', '2018', 371, 'http://ajbuilds.uk/repo/'), 
(05,'TeslaBuilds_Repo', 'Aeon_Tesla', '2018', 150, 'http://theteslabuilds.com'),
(06,'SupremeBuilds_Repo', 'Titanium', '2018', 120, 'http://repo.supremebuilds.com'),
(07,'DurexWizard_Repo', 'Durex', '2018', 470, 'http://www.drxbld.com/wiz/'),
(08,'NoLimitsWizard_Repo', 'No Limits Magic', '2018', 285, 'http://www.nolimitswiz.appboxes.co/'),
(09,'KodiGeeksWizard_Repo', 'Xenon', '2018', 405, 'http://repo.kodigeeks.com/'),
(10,'FireTvGuruWizard_Repo', 'Fire Tv Guru', '2018', 335, 'http://firetvguru.net/fire'),
(11,'Genie TV Repo Wizard', 'Equinox', '2018', 410, 'http://genietv.co.uk/repo/'),
(12,'Misfit Mods Repo', 'Atomic Reborn', '2018', 410, 'http://misfitmods.com/mmwiz/'),
(13,'Warlock Wizard', 'Warlock', '2018', 100, 'http://warlockmedia.eu/warlockwizard/'),
(14,'Wookie Repo and Wizard', 'Wookie', '2018', 200, 'http://wizwookiespm.com'),
(15,'Fire TV Guru', 'Pulse CCM', '2018', 182, 'http://firetvguru.net/fire');


CREATE TABLE if not exists user_info 
( user_id int(5), 
name_f varchar(46),
name_l varchar(46), 
username varchar(46),
email  varchar(255),
age int(2), 
signal_strength varchar(10), 
location varchar(76) 
);

INSERT INTO user_info
(user_id, name_f, name_l, username, email, age, signal_strength, location)
VALUES (01, 'George', 'Matthews', 'GMAC', '26', 'fair', 'Nashville, Tennessee 37209'),
(02,'Taylor', 'Smith', 'TaTa', 23, 'Memphis, Tennessee 38016'),
(03,'Damon', 'Stealth', 'D-Stealth', 34, 'Atlanta, Georgia 30309 '),
(04, 'Aubree_', 'Ronte', 'AJ', 37, 'Lexington, Kentucky 40510'), 
(05,'Tesla', 'Aeon', 'Avenon', 25, 'Cleveland, Ohio 44105'),
(06,'Solomon', 'Titius', 'Supreme', 20, 'Accra, Ghana 00233 '),
(07,'Victoria', 'Durex', 'Rosie', 27, 'Cleveland, Ohio 44105'),
(08,'Madonna', 'Nonless', 'May', 25, 'Cleveland, Ohio 44105'),
(09,'Rashad', 'Xenon', 'Shad', 40, 'Cleveland, Ohio 44105'),
(10,'Teresa', 'Fire ', 'Tree', 33, 'Cleveland, Ohio 44105'),
(11,'Alex', 'Equinox', 'Monte', 41, 'Lexington, Kentucky 40510'),
(12,'Caiden', 'Reborn', 'K.K.', 20, 'Lexington, Kentucky 40510'),
(13,'Mario', 'Warlock', 'Rio', 35, 'Lexington, Kentucky 40510'),
(14,'Steven', 'Wookie', 'Wookie', 20, 'Lexington, Kentucky 40510'),
(15,'Amanda', 'Pulse', 'Mandi', 18, 'Lexington, Kentucky 40510');


CREATE TABLE IF NOT EXISTS Clients (
ClientNo INT NOT NULL,
First_Name VARCHAR (45) NULL,
Last_Name VARCHAR (45) NULL
);

INSERT INTO Clients
VALUES (16, 'Fohn', 'Havis'), (12,'Rohn', 'Wavis'),
(16,'Fohn', 'Qavis'), (14, 'Gohn', 'Tavis'), (12,'Dillo', 'Tanks');

CREATE VIEW ourView2 AS
SELECT *
FROM clients
WHERE ClientNo = 16;

CREATE VIEW ourView AS
SELECT *
FROM clients
WHERE ClientNo = 16;


SELECT * 
FROM ourView;

SELECT * 
FROM ourView2;


SELECT * 
FROM data_location;

SET SQL_SAFE_UPDATES = 0;

INSERT INTO Clients VALUES (NULL, 'Fillo', 'Uanks');

UPDATE Clients
SET ClientNo = 15
WHERE ClientNo = 12;

UPDATE Clients
SET ClientNo = 12
WHERE ClientNo = NULL ;

DELETE FROM Clients
WHERE ClientNo = 12;

DROP ourView
DROP Clients;

CREATE TABLE IF NOT EXISTS Clients2 (
ClientNo INT NOT NULL,
First_Name VARCHAR (45) NULL,
Last_Name VARCHAR (45) NULL
);

INSERT INTO builds_id 
(id, wizard_name, build_name, age_of_build, network_number_bit_size, network_location)
VALUES (01, 'OneNation_Repo', 'Lobo', '2017', '156', 'http://www.onenation.info/Repo/'),
(02,'TurboTv_Repo', 'Turbo', '2017', 260, 'http://turbojtv.com/repo/'),
(03,'SG_Repo', 'Stealth', '2018', 264, 'http://sgwizard.96.lt/'),
(04, 'AJ_Repo', 'Xontech_Light', '2018', 371, 'http://ajbuilds.uk/repo/'), 
(05,'TeslaBuilds_Repo', 'Aeon_Tesla', '2018', 150, 'http://theteslabuilds.com'),
(06,'SupremeBuilds_Repo', 'Titanium', '2018', 120, 'http://repo.supremebuilds.com'),
(07,'DurexWizard_Repo', 'Durex', '2018', 470, 'http://www.drxbld.com/wiz/'),
(08,'NoLimitsWizard_Repo', 'No Limits Magic', '2018', 285, 'http://www.nolimitswiz.appboxes.co/'),
(09,'KodiGeeksWizard_Repo', 'Xenon', '2018', 405, 'http://repo.kodigeeks.com/'),
(10,'FireTvGuruWizard_Repo', 'Fire Tv Guru', '2018', 335, 'http://firetvguru.net/fire'),
(11,'Genie TV Repo Wizard', 'Equinox', '2018', 410, 'http://genietv.co.uk/repo/'),
(12,'Misfit Mods Repo', 'Atomic Reborn', '2018', 410, 'http://misfitmods.com/mmwiz/'),
(13,'Warlock Wizard', 'Warlock', '2018', 100, 'http://warlockmedia.eu/warlockwizard/'),
(14,'Wookie Repo and Wizard', 'Wookie', '2018', 200, 'http://wizwookiespm.com'),
(15,'Fire TV Guru', 'Pulse CCM', '2018', 182, 'http://firetvguru.net/fire');

CREATE VIEW ourView2 AS
SELECT *
FROM clients
WHERE ClientNo = 16;

CREATE VIEW builds_idView AS
SELECT *
FROM builds_id;


INSERT INTO Clients2
VALUES (16, 'Fohn', 'Havis'), (12,'Rohn', 'Wavis'),
(16,'Fohn', 'Qavis'), (14, 'Gohn', 'Tavis'), (12,'Dillo', 'Tanks');

CREATE VIEW ourView2 AS
SELECT *
FROM clients
WHERE ClientNo = 16;

INSERT INTO Clients2
VALUES (16, 'Fohn', 'Havis'), (12,'Rohn', 'Wavis'),
(16,'Fohn', 'Qavis'), (14, 'Gohn', 'Tavis'), (12,'Dillo', 'Tanks');

CREATE VIEW ourView2 AS
SELECT *
FROM clients
WHERE ClientNo = 16;

SELECT *
From builds_id;
 
