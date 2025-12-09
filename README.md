# nested-relationship-ta-certo-agora-
class EventoSerializer(serializers.ModelSerializer):

# NESTED RELATIONSHIP:

participante = ParticipanteSerliarizer(many=True, read_only=True)

# HiperLinked Related Fild

participante = serliarizers.HiperlinkedRelatedField(many=True, read_only=True, view_name='paticipante-detail')

# Primary Key Related Fild

participante = serliarizers.PrimaryKeyRelatedFild(many=True, read_only=True) (#comentario#)nenhua ou muitas 
