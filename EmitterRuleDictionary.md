# Emitter Rule Properties
## Header
**Name** - Unique Emitter Rule name, used to target it in EffectRuleDictionary

**Unknown10** - ? -

**Unknown628** - bit - looping?

## ============================================================
# Domain1
CreationDomain defines properties of the area where new particles are spawned.
_UNCONFIRMED_ - Position seems to be relative to the previous particle?

**Type** - string -  _Box, Cylinder, Sphere_

**Unknown10** - flag? - _0x0, 0x100, 0x101, 0x1_

**Unknown258** - ? - _2 or 2.1_

## KeyframeProperty0
### ptxCreationDomain:m_positionKFP

**Unknown0**

**Unknown4**

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

## KeyframeProperty1
### ptxCreationDomain:m_rotationKFP


**Unknown0**

**Unknown4**

**Unknown10** - X

**Unknown14** - Y

**Unknown18** - Z

**Unknown1C**

	<KeyframeProperty1>
		<Name>ptxCreationDomain:m_rotationKFP</Name>
		<Unknown6C value="20992"/>
		<Keyframes/>
	</KeyframeProperty1>

## KeyframeProperty2
### ptxCreationDomain:m_sizeOuterKFP

**Unknown0**

**Unknown4**

**Unknown10** - X

**Unknown14** - Y

**Unknown18** - Z

**Unknown1C**

	<KeyframeProperty2>
		<Name>ptxCreationDomain:m_sizeOuterKFP</Name>
		<Unknown6C value="21248"/>
		<Keyframes/>
	</KeyframeProperty2>

## KeyframeProperty3
### ptxCreationDomain:m_sizeInnerKFP

**Unknown0**

**Unknown4**

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
# Domain2
TargetDomain defines the area where particles tend to move. Their agility, speed and actual direction are also dependant on their own properties, and particles may die before reaching target domain if their lifetime is too short.

**Type** - string -  _Box, Cylinder, Sphere_

**Unknown10** - flag? - _0x0, 0x100, 0x101, 0x1_

**Unknown258** - ? - _2 or 2.1_

## KeyframeProperty0
### ptxTargetDomain:m_positionKFP

**Unknown0**

**Unknown4**

**Unknown10** - X

**Unknown14** - Y

**Unknown18** - Z

**Unknown1C**

	<KeyframeProperty0>
		<Name>ptxTargetDomain:m_positionKFP</Name>
		<Unknown6C value="20736"/>
		<Keyframes/>
	</KeyframeProperty0>

## KeyframeProperty1
### ptxTargetDomain:m_rotationKFP

**Unknown0**

**Unknown4**

**Unknown10** - X

**Unknown14** - Y

**Unknown18** - Z

**Unknown1C**

	<KeyframeProperty1>
		<Name>ptxTargetDomain:m_rotationKFP</Name>
		<Unknown6C value="20992"/>
		<Keyframes/>
	</KeyframeProperty1>

## KeyframeProperty2
### ptxTargetDomain:m_sizeOuterKFP

**Unknown0**

**Unknown4**

**Unknown10** - X

**Unknown14** - Y

**Unknown18** - Z

**Unknown1C**

	<KeyframeProperty2>
		<Name>ptxTargetDomain:m_sizeOuterKFP</Name>
		<Unknown6C value="21248"/>
		<Keyframes/>
	</KeyframeProperty2>

## KeyframeProperty3
### ptxTargetDomain:m_sizeInnerKFP

**Unknown0**

**Unknown4**

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
# Domain3
Third Domain is only used as Attractor Domain, isn't present in Emitter Rule if not required.

**Type** - string -  _Attractor_

**Unknown10** - flag? - _0x0, 0x100, 0x101, 0x1_

**Unknown258** - ? - _2 or 2.1_

## KeyframeProperty0

### ptxAttractorDomain:m_positionKFP


**Unknown0**

**Unknown4**

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

## KeyframeProperty1
### ptxAttractorDomain:m_rotationKFP

**Unknown0**

**Unknown4**

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
		
## KeyframeProperty2
### ptxAttractorDomain:m_sizeOuterKFP

**Unknown0**

**Unknown4**

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
		
## KeyframeProperty3
### ptxAttractorDomain:m_sizeInnerKFP

**Unknown0**

**Unknown4**

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
