# linked-blog-starter-md
These are the markdown files for the [linked-blog-starter](https://github.com/matthewwong525/linked-blog-starter) repository

1. Education: Back to Focus

	Students with attention Attention-Deficit Hyperactivity Disorder(ADHD) tend to get distracted easily or struggle focusing in class. ADHD commonly gets misinterpreted as laziness or poor discipline, leading to underdiagnosis. Conventional intervention is typically a one-on-one session, but this can draw unwanted peer attention and judgements. Back to focus presents an alternative, non-disruptive, desk-integrated tool that will help students directly from their desks. By installing a custom foot pedal equipped with Inertia Measurement Unit (IMU), the system will be able to track leg movements. When movements indicate restlessness or boredom, a vibration will be sent to the chair that will buzz softly the cue them back to focus.

	Background
		One of the most common neurodevelopment conditions affecting academic performance is Attention-Deficit Hyperactivity Disorder(ADHD). Most learning environment aim to help these students.
		``
		In typical Philippine public schools, classrooms are often densely populated. Making it difficult for teachers to provide personalized attention to students. Students with ADHD often struggle with focusing in class, usually manifesting as restlessness or zoning out. Current interventions involve one-on-one out of classroom session with the student. However, this can attract unwanted attention thus disrupting learning and academic performance. In addition, fidget tools that require the hand to use, takes away the hands of the students to write.
		To address this, Project Back to Focus introduces an under-desked foot pedal that will monitor and track foot movements and provide private feedbacks. Allowing students to self-regulate seamlessly without disrupting the class from their own seats.
		
		
	
	
	
	Significance of the study
		To Neurodivergent students: it provides an alternative way to help them focus in class without disruption and is low profile.
		To Teachers: It reduces the need to constantly monitor or manually call out distracted students, minimizing the disruption and the need for one-on-one treatment sessions.
		

	System Architecture:
		A custom foot pedal that is housed under a desk. It is Arduino powered connected to a IMU and a vibration motor that is rested in the chair.

	How it works:The IMU continuously track the angular frequency of students foot tapping or fidgetting.

	Condition A(Hyperactivity): If the foot movements frequency exceeds 5 Hz for more than 10 seconds, then the Arduino identifies it as Hyperactivity(restlessness/impatience)

	Condition B(Zoning out):
		If foot movements stops for more than 180 seconds (5 minutes) during an active lecture, then Arduino identifies it as zoning out.

	Response: The system will send a low-frequency vibration that lasts for 1.5 seconds that will cue the student back to focus.

	Data collection and Testing: The project will utilize an ABAB withdrawal research in general classroom settings that will evaluate the percentage gain in attention when the device is active versus inactive.
		
	RRL
	Behavioral studies show that tactile fidgets gains 45% to 55% in overall instructional focus among elementary students. While existing fidget items (like spinners or stress balls) works, it occupies the hand of the student making them unable to write and get distracted, a lower-body mechanism keeps the hands completely free for academic work while reducing visible disruption.
	
	
	References
	https://www.naset.com/publications/adhd-series/examining-the-effectiveness-of-fidgets-on-attention-of-elementary-students-with-adhd/


	

	There is a foot pedal under the table where the students foot will be placed. The pedal will track the movement of the student, if it senses that the movement becomes to frantic (signaling boredom/high anxiety/impatience) or stops for too long (signaling zoning), a Vibration on a chair will buzz softly to cue them back into focus.

	Students with the symptoms or diagnosed with ADHD are the primary beneficiaries of our project. It is a alternative to help stay class without any outside help.




	Keeping students with hyperactive or attention-deficit tendencies engaged without disrupting the rest of the classroom.



	The Idea: A silent, under-desk "fidget pedal" or foot rocker that tracks micro-movements and uses subtle haptic (vibration) feedback to help students self-regulate.



	How it works: An MPU6050 Accelerometer/Gyroscope is attached to a small, spring-loaded foot pedal under the desk. Instead of restricting movement, the Arduino tracks the cadence of the rocking. If the movement becomes frantic (signaling high anxiety/boredom) or stops entirely for too long (signaling zoning out), a gentle Vibration Motor on the student's wristband or chair buzzes softly to gently cue them back to focus.

	https://www.mdpi.com/2076-3425/13/12/1728
	https://link.springer.com/article/10.1007/s10882-018-9623-z?fromPaywallRec=true
	



### 2. EDUCATION: The "Unplugged" Interactive Physics/Chemistry Lab Mesh
- **The Specific Problem:** Millions of public school students in remote, off-grid _bayan_ (rural areas) lack science laboratories and computers. While they have access to static textbooks, they cannot experience real, hands-on science experiments.

- **The "I Never Thought of That" Twist:** **Physical-to-Data Sandbox Blocks.**

- **The Arduino Setup:** Instead of a computer simulation, build a kit of low-cost, rugged "Smart Blocks" powered by Arduino. Each block contains an embedded sensor (e.g., an accelerometer, color sensor, or temperature probe) and an e-paper display (which requires almost zero power and works in direct sunlight).

- **The Action:** When students snap different blocks together like physical LEGO bricks, the blocks talk to each other over a local peer-to-peer network (no internet required). If they shake an "acceleration block" or dip a "thermal block" into water, the exact laws of physics or data reactions render directly on the block's e-paper screen. It brings a dynamic science lab into communities that have zero electricity.


**Project LINYA: An Arduino-Based Lane-Splitting Space Matrix and Warning Indicator for Blind Intersection Motorcycle Safety**

### 🔍 1. Executive Summary

Most cities in the Philippines experience high densities of motorcycle traffic, where riders frequently practice "overtaking" . A major hazard occurs at narrow, blind intersections where larger vehicles (trucks, SUVs) completely block a turning driver's line of sight, preventing them from seeing a high-speed motorcycle until an accident is inevitable. Project Side-View addresses this large vehicles blind spot by mounting an autonomous Arduino monitoring node onto roadside utility poles at high-risk intersections or on the vehicles itself. Using sensors, the system continuously maps the spatial gap between vehicle lanes. If a motorcycle is detected moving through a blind corridor simultaneously with a vehicle executing a turn, the system computes an immediate collision threat and triggers high-visibility road-surface laser projections to visually alert both operators before they cross paths.



###  2. Background

The transportation in the Philippines has seen an exponential rise in two-wheeled motor vehicles, making motorcycles the primary mode of daily commuting for millions. Due to severe traffic, riders frequently utilize "overtaking" through the tight spaces between slow-moving or stationary lanes of cars and trucks.

While overtaking saves time for motorcycles, it introduces severe safety vulnerabilities, particularly at blind intersections. When large vehicles like buses, trucks, or SUVs occupy the primary lanes, they create a complete visual blockage. A driver attempting to execute a turn at an intersection cannot see a filtering motorcycle approaching through the lane gap until the moment of impact. Standard vehicle-mounted blind-spot indicators are often too slow or uncalibrated for low-profile, fast two-wheelers, leading to high accident rates at narrow crossroads.

Rather than relying on expensive, vehicle-dependent radar systems, transportation safety can be significantly enhanced through smart, affordable indicators. Project Side-view addresses this problem by introducing an infrastructure-based, high-speed laser sensor. Placed at high-conflict blind corners or at vehicle itself, this automated system calculates collision probabilities in real time, projecting dynamic visual warnings directly onto the asphalt if it is mounted at an infrastructure, if it is mounted to a vehicle it will send a signal to the driver to secure vulnerable motorcycle commuters.

### 3.Methodology

- **Methodology/Logic Flow:**
	
    - The Arduino monitors distance changes to recognize small profiles (motorcycles) traveling within the lane bounds.
        
    - **Predictive Calculation:** If the system calculates a vehicle lane occupancy change (indicating a turn into the intersection) while sensor registers a fast-approaching motorcycle profile within a 15-meter zone, a high-probability conflict is flagged.
        
    - **Response:** The system immediately activates an intense, downward-projected visual grid onto the asphalt directly in front of the turning vehicle's windshield line-of-sight and activates an audio siren facing the oncoming rider.
        

### 4. Review of Related Literature (RRL)

In addressing the vulnerability of motorcycle commuters, **Chang et al. (2023)** developed an effective Proactive Blind Spot Warning (PBSW) system specifically for motorcycles using a dual-lens stereo camera system combined with a cloud-based YOLOv4 model to calculate real-time relative distances and warn riders when they enter a larger vehicle’s blind spot. While their research successfully demonstrated a high position detection accuracy of 92.82%, the authors noted that there is a 0.5 seconds round trip delay. Their approach focused more on vehicle to vehicle calculations, which requires a complex capturing hardware. Project Side view instead of only being vehicle mounted it can also be mounted to infrastructure, it also pivots away from image-based processing and instead using a laser distance sensor node. This completely removes cloud network latency. 
### 5. Significance of the Study

- **To Motorcycle Commuters:** It provides an immediate layer of safety for vulnerable road users against overtaking accidents, actively protecting them from collision blind spots caused by larger vehicles.
    
- **To Drivers:** It removes the anxiety and high-risk legal/financial liabilities associated with accidental intersection collisions by providing highly visible warnings right in their line of sight.
    
- **To Traffic Management and LGUs:** It offers local government units a highly scalable, low-cost smart solution to reduce accident rates without relying on multi-million peso infrastructure overhauls.
    

### 6. Reference List

- Real-time vision-based blind spot warning system: Experiments with motorcycles in daytime/nighttime conditions
	https://link.springer.com/article/10.1007/s12239-013-0013-3
-