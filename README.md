# leetcode_Analisis_de_algoritmos
Ejercicios semanales

class Solution:

    def twoSum(self, nums: List[int], target: int) -> List[int]:
        """
        Encuentra los índices de dos números en una lista que sumen un valor dado.

        se usa una tabla hash para lograr una complejidad de tiempo lineal O(n),
        almacenando los valores visitados y sus índices correspondientes.

        Args:
            nums (List[int]): Una lista de números enteros.
            target (int): El valor objetivo de la suma.

        Returns:
            List[int]: Una lista con los dos índices de los números que suman el target.
        """

        prevMap = {}
        for i, n in enumerate(nums):
            diff = target - n

            if diff in prevMap:
                return [prevMap[diff], i]
            prevMap[n] = i
