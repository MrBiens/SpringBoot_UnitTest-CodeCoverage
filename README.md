SpringBoot_UnitTest-CodeCoverage

Jacoco Plugin
<plugin>
				<groupId>org.jacoco</groupId>
				<artifactId>jacoco-maven-plugin</artifactId>
				<version>0.8.12</version>
				<executions>
					<execution>
						<goals>
							<goal>prepare-agent</goal>
						</goals>
					</execution>
					<execution>
						<id>report</id>
						<phase>prepare-package</phase>
						<goals>
							<goal>report</goal>
						</goals>
					</execution>
				</executions>
				<configuration>
					<!-- Loại trừ những packega không tính vào test jacoco : report-->
					<excludes>
						<exclude>com.vn.sbit.idenfity_service/dto/**</exclude>
						<exclude>com.vn.sbit.idenfity_service/mapper/**</exclude>
						<exclude>com.vn.sbit.idenfity_service/entity/**</exclude>
						<exclude>com.vn.sbit.idenfity_service/configuration/**</exclude>
					</excludes>
				</configuration>
			</plugin>

H2 Databas -DBLocal
	<dependency>
			<groupId>com.h2database</groupId>
			<artifactId>h2</artifactId>
			<version>2.2.224</version>
			<scope>test</scope>
		</dependency>
  
LocalDate convert to JSON		
    <!--  -->
<dependency>
    <groupId>com.fasterxml.jackson.datatype</groupId>
    <artifactId>jackson-datatype-jsr310</artifactId>
</dependency>

  	<!-- Test method Authorize-->

Security test 
		<dependency>
			<groupId>org.springframework.security</groupId>
			<artifactId>spring-security-test</artifactId>
			<scope>test</scope>
		</dependency>




