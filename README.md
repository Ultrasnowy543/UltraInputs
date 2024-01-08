This Is UltraInputs A Unity XR Input System Meant For Oculus Here Is How To Use It:

To Start Using UltraInputs You Will Need To Import It Then In A Script Add This Using Statement At The Top:
using Ultrasnowy543.ultraInputs;

To Get Something Like The Trigger Being Pushed Down On The Left Hand You Would Do:
UltraInputs.GetBool(HandChoice.LeftHand, InputReferenceBool.TriggerPress);
This Will Return True If The Trigger On The Left Hand Is Pressed And False If It Is Not

To Get Something Like The Amount That The Trigger Has Been Pushed Down On The Right Hand You Would Do:
UltraInputs.GetFloat(HandChoice.RightHand, InputReferenceFloat.TriggerFloat);
This Will Return How Far Down The Trigger Has Been Pushed Down On The Right Hand A Value That Is Between 0.0 And 1.0

To Get Something Like The Velocity Of The Left Hand You Would Do:
UltraInputs.GetVector3(HandChoice.LeftHand, InputReferenceVector3.Velocity);
This Will Return The Velocity Of The Left Hand
WARNING:
If You Get The Controller Rotation From This It Will Return It's Euler Angles Use Quaternion.Euler() To Convert It Back To A Quaternion

To Vibrate The Right Hand For 0.2 Seconds With An Amplitude Of 0.5 You Would Do:
UltraInputs.SendHapticVibrations(HandChoice.RightHand, 0.5f, 0.2f);
