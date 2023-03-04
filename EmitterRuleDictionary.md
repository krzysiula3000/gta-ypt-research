# Emitter Rule Properties
## Header
**Name** - Unique Emitter Rule name, used to target it in EffectRuleDictionary.  
**Unknown10** - ? -  
**Unknown628** - bit - looping?  

### Unknown0 & Unknown4
These settings are universal for all keyframes in all KFP types.  
_UNCONFIRMED_ - define timeline position and lengh of each frame.  
Will be omitted in the following sections.

## ============================================================
## Domain1
CreationDomain defines properties of the area where new particles are spawned.
_UNCONFIRMED_ - Position seems to be relative to the previous particle?

**Type** - string -  _Box, Cylinder, Sphere_  
**Unknown10** - flag? - _0x0, 0x100, 0x101, 0x1_  
**Unknown258** - ? - _2 or 2.1_  

### KeyframeProperty0
### ptxCreationDomain:m_positionKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty0>
		<Name>ptxCreationDomain:m_positionKFP</Name>
		<Unknown6C value="20736"/>
		<Keyframes>
			<Item>
				<Unknown0 value="0"/>
				<Unknown4 value="0"/>
				<Unknown10 value="-0.5"/>
				<Unknown14 value="-1"/>
				<Unknown18 value="-0.85"/>
				<Unknown1C value="0"/>
			</Item>
		</Keyframes>
	</KeyframeProperty0>

### KeyframeProperty1
### ptxCreationDomain:m_rotationKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty1>
		<Name>ptxCreationDomain:m_rotationKFP</Name>
		<Unknown6C value="20992"/>
		<Keyframes/>
	</KeyframeProperty1>

### KeyframeProperty2
### ptxCreationDomain:m_sizeOuterKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty2>
		<Name>ptxCreationDomain:m_sizeOuterKFP</Name>
		<Unknown6C value="21248"/>
		<Keyframes/>
	</KeyframeProperty2>

### KeyframeProperty3
### ptxCreationDomain:m_sizeInnerKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty3>
		<Name>ptxCreationDomain:m_sizeInnerKFP</Name>
		<Unknown6C value="21504"/>
		<Keyframes/>
	</KeyframeProperty3>

## ============================================================
## Domain2
TargetDomain defines the area where particles tend to move. Their agility, speed and actual direction are also dependant on their own properties, and particles may die before reaching target domain if their lifetime is too short.

**Type** - string -  _Box, Cylinder, Sphere_  
**Unknown10** - flag? - _0x0, 0x100, 0x101, 0x1_  
**Unknown258** - ? - _2 or 2.1_  

### KeyframeProperty0
### ptxTargetDomain:m_positionKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty0>
		<Name>ptxTargetDomain:m_positionKFP</Name>
		<Unknown6C value="20736"/>
		<Keyframes/>
	</KeyframeProperty0>

### KeyframeProperty1
### ptxTargetDomain:m_rotationKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty1>
		<Name>ptxTargetDomain:m_rotationKFP</Name>
		<Unknown6C value="20992"/>
		<Keyframes/>
	</KeyframeProperty1>

### KeyframeProperty2
### ptxTargetDomain:m_sizeOuterKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty2>
		<Name>ptxTargetDomain:m_sizeOuterKFP</Name>
		<Unknown6C value="21248"/>
		<Keyframes/>
	</KeyframeProperty2>

### KeyframeProperty3
### ptxTargetDomain:m_sizeInnerKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty3>
		<Name>ptxTargetDomain:m_sizeInnerKFP</Name>
		<Unknown6C value="21504"/>
		<Keyframes/>
	</KeyframeProperty3>

## ============================================================
## Domain3
Third Domain is only used as Attractor Domain, isn't present in Emitter Rule if not required.

**Type** - string -  _Attractor_  
**Unknown10** - flag? - _0x0, 0x100, 0x101, 0x1_  
**Unknown258** - ? - _2 or 2.1_  

### KeyframeProperty0
### ptxAttractorDomain:m_positionKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty0>
		<Name>ptxAttractorDomain:m_positionKFP</Name>
		<Unknown6C value="62464"/>
		<Keyframes>
			<Item>
				<Unknown0 value="0" />
				<Unknown4 value="0" />
				<Unknown10 value="0" />
				<Unknown14 value="0" />
				<Unknown18 value="2.6" />
				<Unknown1C value="0" />
			</Item>
		</Keyframes>
	</KeyframeProperty0>

### KeyframeProperty1
### ptxAttractorDomain:m_rotationKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty1>
		<Name>ptxAttractorDomain:m_rotationKFP</Name>
		<Unknown6C value="62720"/>
		<Keyframes>
			<Item>
				<Unknown0 value="0" />
				<Unknown4 value="0" />
				<Unknown10 value="90" />
				<Unknown14 value="-0.322393" />
				<Unknown18 value="1.074622" />
				<Unknown1C value="0" />
			</Item>
		</Keyframes>
	</KeyframeProperty1>
		
### KeyframeProperty2
### ptxAttractorDomain:m_sizeOuterKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty2>
		<Name>ptxAttractorDomain:m_sizeOuterKFP</Name>
		<Unknown6C value="62976"/>
		<Keyframes>
			<Item>
				<Unknown0 value="0" />
				<Unknown4 value="0" />
				<Unknown10 value="80.03211" />
				<Unknown14 value="0" />
				<Unknown18 value="0" />
				<Unknown1C value="0" />
			</Item>
		</Keyframes>
	</KeyframeProperty2>
		
### KeyframeProperty3
### ptxAttractorDomain:m_sizeInnerKFP

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C**  

	<KeyframeProperty3>
		<Name>ptxAttractorDomain:m_sizeInnerKFP</Name>
		<Unknown6C value="63232"/>
		<Keyframes>
			<Item>
				<Unknown0 value="0" />
				<Unknown4 value="0" />
				<Unknown10 value="21.97635" />
				<Unknown14 value="5.264501" />
				<Unknown18 value="0" />
				<Unknown1C value="0" />
			</Item>
		</Keyframes>
	</KeyframeProperty3>

## ============================================================
## KeyframeProperties
All properties not related to three main domains are defined in this section.

### Example structure
	<Item>
		<Name>ptxEmitterRule:m_spawnRateOverTimeKFP</Name>
		<Unknown6C value="18176"/>
		<Keyframes>
			<Item>
				<Unknown0 value="0"/>
				<Unknown4 value="0"/>
				<Unknown10 value="50"/>
				<Unknown14 value="65"/>
				<Unknown18 value="0"/>
				<Unknown1C value="0"/>
			</Item>
		</Keyframes>
	</Item>

**Unknown6C** - KFP index, increases by 256 every KFP entry. _UNCONFIRMED_ - Not important for the game?  

### ptxEmitterRule:m_playbackRateScalarKFP
Global modifier to the playback speed of particles emitted by this emitter.  
Can be used to speed up or slow down particles visually without affecting their range and lifetime.

**Unknown10** - Playback rate modifier, base value = 1  
**Unknown14** - _Usually 0 or 0.01_  
**Unknown18** - _Usually 0 or 0.01_  
**Unknown1C** - _Usually 0 or 0.01_  

### ptxEmitterRule:m_spawnRateOverTimeKFP

**Unknown10** - Min  
**Unknown14** - Max  
**Unknown18** - Unknown  
**Unknown1C** - _Always 0_  

### ptxEmitterRule:m_spawnRateOverDistKFP

**Unknown10** - Min  
**Unknown14** - Max  
**Unknown18** - Unknown  
**Unknown1C** - _Always 0_  

### ptxEmitterRule:m_particleLifeKFP
Lifetime of each individual particle  
_UNCONFIRMED_ - in frames?

**Unknown10** - Min  
**Unknown14** - Max  
**Unknown18** - _Always 0.01_  
**Unknown1C** - _Always 0.01_  

### ptxEmitterRule:m_speedScalarKFP
Speed multiplier for all particles from this emitter

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C** - _Always 0_  

### ptxEmitterRule:m_sizeScalarKFP
Size multiplier for all particles from this emitter

**Unknown10** - X  
**Unknown14** - Y  
**Unknown18** - Z  
**Unknown1C** - _Always 0_  

### ptxEmitterRule:m_accnScalarKFP
Acceleration multiplier for all particles from this emitter

**Unknown10** - Min  
**Unknown14** - Max  
**Unknown18** - Unknown  
**Unknown1C** - _Always 0_  

### ptxEmitterRule:m_dampeningScalarKFP

**Unknown10** - X?  
**Unknown14** - Y?  
**Unknown18** - Z?  
**Unknown1C** - Unknown

### ptxEmitterRule:m_matrixWeightScalarKFP
_Rarely used_

**Unknown10** - Unknown  
**Unknown14** - Unknown  
**Unknown18** - Unknown  
**Unknown1C** - Unknown

### ptxEmitterRule:m_inheritVelocityKFP

**Unknown10** - Unknown  
**Unknown14** - Unknown  
**Unknown18** - _Always 0_    
**Unknown1C** - _Always 0_  
